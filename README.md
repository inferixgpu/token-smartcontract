# Inferix Token Contracts

This repository contains the smart contracts for the **Testnet phase** of the [Inferix](https://inferix.io/) project. These contracts enable users to interact with the IoTeX Testnet environment and test a simple ERC20 token implementation.

## Project Overview

Inferix aims to decentralize verification processes. This Testnet phase focuses on:

- Testing the functionality and robustness of the ERC20 token contract.
- Preparing for the Mainnet launch by gathering feedback and ensuring security.

## Features

- **ERC20 Token Contract**: Implements a basic ERC20 token for the Testnet phase.
- **Test Environment**: Provides a controlled environment to validate contract interactions and performance.

## Repository Structure

- **contracts/**: Contains the Solidity smart contracts.
- **ignition/modules/**: Includes the deployment script `InferixToken.js` for the Testnet phase.
- **test/**: Contains unit tests to ensure contract functionality.
- **hardhat.config.js**: Configuration for the Hardhat development environment.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v20+ recommended)
- [Hardhat](https://hardhat.org/)
- Access to the IoTeX Testnet network

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/inferixgpu/token-contract-testnet.git
   cd token-contract-testnet
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Compile the contracts:

   ```bash
   npx hardhat compile
   ```

4. Run the tests:

   ```bash
   npx hardhat test
   ```

### Deployment

1. Configure the IoTeX Testnet details in `hardhat.config.js`.
2. Deploy the ERC20 token contract using the Ignition module:

   ```bash
   npx hardhat ignition deploy ignition/modules/InferixToken.js --network iotex_testnet
   ```

### Interaction

Use the provided scripts in the `ignition/modules/` directory to interact with the deployed ERC20 token contract, such as transferring tokens or checking balances.

## Testing

The Testnet phase includes comprehensive tests to ensure the contracts function as expected. Run the test suite with:

```bash
npx hardhat test
```

## Feedback

As this is the Testnet phase, feedback is crucial for identifying issues and improving the contracts. Please report any bugs or suggestions via GitHub issues or contact us directly.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contribution

Contributions are welcome! Open an issue or pull request with your ideas or improvements.

## Contact

For more information, visit [Inferix](https://inferix.io) or contact us via [contact@inferix.io](mailto:contact@inferix.io).

