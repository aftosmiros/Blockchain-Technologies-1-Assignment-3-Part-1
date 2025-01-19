# AITU_SE2324_KV - ERC-20 Token Contract

## Overview

This project implements an ERC-20 token contract named `AITU_SE2324_KV` with the following features:

- **Initial Supply:** Configurable at deployment.
- **Standards:** Implements the ERC-20 token standard.
- **Additional Features:**
  - Retrieve details of the latest transaction, including sender, receiver, amount, and timestamp.
  - Display the timestamp of the latest transaction in a human-readable format.
  - Retrieve the sender and receiver addresses of the latest transaction.

## Features

### Key Functions
- `transfer(address _to, uint256 _value)`:
  - Transfers tokens to the specified address and updates the `latestTransaction` record.

- `transferFrom(address _from, address _to, uint256 _value)`:
  - Transfers tokens from one address to another and updates the `latestTransaction` record.

- `getLatestTransactionTimestamp()`:
  - Returns the timestamp of the latest transaction in a human-readable format (e.g., `1 days, 2 hours, 3 minutes, 4 seconds ago`).

- `getTransactionSender()`:
  - Retrieves the sender address of the latest transaction.

- `getTransactionReceiver()`:
  - Retrieves the receiver address of the latest transaction.

## Deployment

The contract can be deployed on a testnet using tools like Remix and MetaMask:

1. Deploy the contract in **Remix** using the `Injected Web3` environment.
2. Select the desired testnet (e.g., Goerli) in MetaMask and ensure you have sufficient test ETH for gas fees.
3. Specify the initial supply during deployment.

## Project Repository

### Structure
```
├── contracts
│   └── AITU_SE2324_KV.sol       # ERC-20 token contract
├── README.md                    # Documentation
├── LICENSE                      # License file (optional)
├── screenshots.pdf              # Directory for screenshots or demo images (optional)
├── .gitignore                   # Git ignore file
```

### Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AITU_SE2324_KV.git
   cd AITU_SE2324_KV
   ```

2. Open the contract in Remix:
   - Navigate to `contracts/AITU_SE2324_KV.sol`.
   - Compile the contract with the correct Solidity version (`^0.8.0`).

3. Deploy and interact with the contract.

## Usage

### Example Interaction

- **Deploying the Contract:**
  - Specify the initial token supply in the deployment dialog.

- **Transferring Tokens:**
  - Use the `transfer` function to send tokens to an address.
  - Call `getLatestTransactionTimestamp()` to verify the timestamp of the transaction.

### Screenshots

#### Contract Deployment
![Deployment Screenshot](images/deployment.png)

#### Transaction Interaction
![Transaction Screenshot](images/transaction.png)

## References

- [OpenZeppelin ERC-20 Implementation](https://github.com/OpenZeppelin/openzeppelin-contracts)
- [ERC-20 Token Standard](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/)
- [Remix IDE](https://remix.ethereum.org/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
