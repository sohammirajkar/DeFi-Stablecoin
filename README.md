Certainly! Here's the updated README.md file with instructions tailored for using Forge instead of Truffle:

---

# Decentralized Stable Coin (DSC) Engine

**Author**: Soham Mirajkar

[![GitHub](https://img.shields.io/badge/GitHub-sohammirajkar-blue)](https://github.com/sohammirajkar/DeFi-Stablecoin.git)

## Overview

The Decentralized Stable Coin (DSC) Engine is a minimalistic system designed to create a stablecoin with a 1 token == $1 peg. It operates on the principles of exogenous collateralization, maintaining a dollar peg, and ensuring algorithmic stability. Inspired by systems like DAI, it differs by having no governance, no fees, and being solely backed by WETH (Wrapped Ethereum) and WBTC (Wrapped Bitcoin).

## Key Features

- **Exogenous Collateral**: The system relies on collateral assets such as WETH and WBTC.
- **Dollar Pegged**: Each DSC token is designed to maintain a value equivalent to $1.
- **Algorithmic Stability**: Mechanisms are in place to ensure stability without the need for governance.

## System Requirements

- [Solidity](https://docs.soliditylang.org/en/v0.8.12/installing-solidity.html)
- [Forge](https://github.com/stableunit/forge-cli)

## Testing

The contract has been thoroughly tested using fuzz testing to ensure robustness and reliability. Fuzz testing involves subjecting the contract to a large number of random inputs to uncover vulnerabilities and edge cases.

To run fuzz tests:

1. Install Forge:

    ```bash
    npm install -g @stableunit/forge-cli
    ```

2. Run fuzz tests:

    ```bash
    forge test
    ```

## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/sohammirajkar/DeFi-Stablecoin.git
    ```

2. Install dependencies:

    ```bash
    cd DeFi-Stablecoin
    npm install
    ```

3. Compile contracts:

    ```bash
    forge compile
    ```

4. Deploy contracts:

    ```bash
    forge migrate --network <network_name>
    ```

5. Interact with the contracts through a web interface or directly using the deployed addresses.

## Usage

The core contract `DSCEngine.sol` handles all the logic for minting, redeeming DSC tokens, as well as depositing and withdrawing collateral.

## Acknowledgments

This project is loosely based on the MakerDAO DSS (DAI) system.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This should provide a comprehensive overview of your DeFi stablecoin project, including instructions tailored for using Forge. Let me know if you need further adjustments!
# DeFi-Stablecoin
