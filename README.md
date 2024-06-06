# ETH-AVAX-Project3
Project 3(ERC20)

# Smart Contract Project: MyToken ERC20 Token

## Overview

This project demonstrates the implementation of an ERC20 token named MyToken (OXY) using Solidity. The smart contract includes minting and burning functionalities, where only the contract owner can mint new tokens, and any user can burn their own tokens. This project helps developers understand how to create and manage ERC20 tokens while implementing ownership and basic token operations.

## Features

- **mint(address to, uint256 amount)**: Mints new tokens to a specified address. This function can only be called by the contract owner.
- **burn(uint256 amount)**: Burns a specified amount of tokens from the caller's balance.
- **Initial Supply**: Mints an initial supply of tokens to the contract deployer's address upon deployment.

## Getting Started

### Prerequisites

- [MetaMask](https://metamask.io/) browser extension
- [Remix IDE](https://remix.ethereum.org/) or any Solidity development environment
- Basic knowledge of Solidity and smart contract development

### Deployment and Testing

1. **Open Remix IDE**:
   - Navigate to [Remix IDE](https://remix.ethereum.org/).

2. **Create a New File**:
   - In the "contracts" folder, create a new file named `MyToken.sol` and paste the Solidity code for the smart contract into the new file.

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

5. **Interact with the Contract**:
   - Once deployed, you can interact with the contract through the "Deployed Contracts" section in Remix.
   - Call the contract functions to mint tokens, burn tokens, and check balances.

## Usage

- **mint(address to, uint256 amount)**: Call this function with the recipient address and the amount of tokens to mint. Only the contract owner can execute this function.
- **burn(uint256 amount)**: Call this function with the amount of tokens to burn from the caller's balance.
- **Transfer Tokens**: Use the standard ERC20 `transfer` function to send tokens to another address.
- **Check Balance**: Use the standard ERC20 `balanceOf` function to check the token balance of an address.

## Contract Code

Here's the Solidity code for `MyToken.sol`:

## License

This project is licensed under the MIT License.

