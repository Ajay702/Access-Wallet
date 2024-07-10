# AccessWallet

## Overview

AccessWallet is a Solidity smart contract that allows for controlled access to deposit and withdraw funds. It includes an administrative control to manage allowed users and ensures only authorized users can interact with the contract.

## Description

AccessWallet manages user balances and permissions using Solidity mappings. The contract has an administrator who can grant access to specific users. Authorized users can deposit Ether into their balance and withdraw Ether, provided they have sufficient funds.

# Getting Started

## Deploying the Contract

### Setup

1. **Environment Setup**: Use Remix or another Solidity development environment.
2. **Create Contract File**: Copy the contract code into a file named `AccessWallet.sol`.

### Compiling and Deploying

1. **Compile the Contract**: Ensure the Solidity compiler version is set to `0.8.20`.
2. **Deploy the Contract**: Deploy the contract to your desired Ethereum network (e.g., Rinkeby, Goerli).

## Interacting with the Contract

Once deployed, interact with the contract using Ethereum wallets or scripting:

- **Allow User**: Only the contract admin can allow users to interact with the contract using the `allowUser` function.
  Example: `allowUser("0xUserAddress")`

- **Deposit Funds**: Allowed users can deposit Ether into their balance using the `deposit` function.
  Example: Send Ether to the contract address with sufficient gas.

- **Withdraw Funds**: Allowed users can withdraw Ether from their balance using the `withdraw` function.
  Example: `withdraw(100)` to withdraw 100 Wei.

## Help

### Common Issues

- **Permission Errors**: Ensure users are allowed via the `allowUser` function before depositing or withdrawing.

### Command for Help

For assistance or more information, refer to Solidity documentation or Ethereum development resources.

## Authors

- **Ajay702**

## License

This project is licensed under the MIT License.
