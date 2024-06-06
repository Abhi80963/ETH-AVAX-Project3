# ETH-AVAX-Project3
Project 3(ERC20)

```markdown
# MyToken ERC20 Token

MyToken (OXY) is an ERC20 token implemented using Solidity. This project demonstrates how to create a basic ERC20 token with minting and burning functionalities, where only the contract owner can mint new tokens, and any user can burn their own tokens.

## Features

- **Minting**: Only the contract owner can mint new tokens to any address.
- **Burning**: Any user can burn their own tokens.
- **Initial Supply**: The initial supply of tokens is minted to the contract deployer's address upon deployment.

## Prerequisites

To deploy and interact with this contract, you need:

- [MetaMask](https://metamask.io/) browser extension
- [Remix IDE](https://remix.ethereum.org/)

## Deployment

1. **Open Remix**: Go to [Remix IDE](https://remix.ethereum.org/).

2. **Create a New File**: In the "contracts" folder, create a new file named `MyToken.sol` and paste the above contract code into it.

3. **Compile the Contract**:
    - Click on the "Solidity Compiler" tab in the left panel.
    - Ensure the compiler version is set to `0.8.0` or higher.
    - Click on the "Compile MyToken.sol" button.

4. **Deploy the Contract**:
    - Go to the "Deploy & Run Transactions" tab.
    - Select "Injected Web3" in the "Environment" dropdown to use MetaMask for deployment.
    - Enter the initial supply of tokens in the constructor arguments field (e.g., `1000000` for 1,000,000 tokens).
    - Ensure `MyToken` is selected in the "Contract" dropdown.
    - Click on the "Deploy" button and confirm the transaction in MetaMask.

## Interacting with the Contract

Once deployed, you can interact with the contract through the "Deployed Contracts" section in Remix.

### Example Interactions

1. **Mint Tokens**:
    - As the owner, call the `mint` function.
    - Provide the recipient address and the amount of tokens to mint.
    ```solidity
    mint("0xRecipientAddress", 1000)
    ```

2. **Burn Tokens**:
    - Call the `burn` function to burn your own tokens.
    ```solidity
    burn(500)
    ```

## License

This project is licensed under the MIT License.

```
