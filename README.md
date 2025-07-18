# 🚀 Sui Arbitrage Bot

A high-performance MEV (Maximal Extractable Value) bot for the Sui blockchain. This bot scans the Sui network for arbitrage opportunities across decentralized exchanges (DEXs), automatically executing profitable trades. 

## Features

- Real-time monitoring of Sui blockchain transactions
- Automated detection of arbitrage opportunities
- Fast execution to maximize profits
- Configurable trading strategies

## Requirements(one of the following):

Recommended:
- **machine**: an 8 CPU/vCPU, 32GB RAM, and 512GB NVMe SSD as a minimum.
- **vemius-node**: a fork of the Sui node with enhanced features for MEV bots. see [vemius-node](https://github.com/xun0n/vemius-node).
- **geyser**: configure in vemius-node to enable MEV features.

Other:
- **web-socket-rpc**: a WebSocket RPC endpoint for Sui.
- **sui-rpc**: a fast Sui RPC endpoint.

## Getting Started

1. **Download the pre-built binary:**  
   You can download the latest release from the [Releases](https://github.com/xun0n/sui-mev/releases) page. 

2. **Generate a operation wallet:**  
   Use suici to create a new wallet for operations:
    ```bash
    suici wallet --keypair /path/to/save create
    ```

3. **Configure your settings:**  
    Edit `config.yaml` with your wallet and strategy preferences.

4. **Deposit SUI tokens:**  
   Ensure your operation wallet has sufficient SUI tokens for transaction fees and trading. For example, 0.1 SUI is recommended.

5. **Run the bot:**
    ```bash
    suici mev --config config.yaml
    ```

## Disclaimer

This software is for educational and research purposes only. Use at your own risk.
