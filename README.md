# Galaxy Explorer (Built for Base)

Galaxy Explorer is a lightweight, read-only tool created for quickly inspecting the Base Sepolia network. With just a few commands, you can verify wallet balances, check network status, and validate contract deployments, all without altering any blockchain data.

---

## Key Features

Galaxy Explorer enables you to:
- **Check Wallet Balances**: View the balance of any wallet on Base Sepolia.
- **Validate Contract Deployments**: Ensure contract deployments are correct with direct Basescan links.
- **Inspect Network Configuration**: Confirm that you are connected to the Base Sepolia network (chainId: 84532).
- **Monitor Blockchain Data**: Review the latest blocks and gas usage.

All actions are read-only, meaning no changes will be made to the blockchain during usage.

---

## How It Works

Galaxy Explorer connects to Coinbase Wallet using the Coinbase Wallet SDK and queries the Base Sepolia network via the viem library. The tool retrieves important blockchain data, such as wallet balances, transaction counts, block details, and gas prices. It provides explorer links to verify the data without making any changes to the blockchain.

The entire process is read-only, ensuring a non-intrusive experience.

---

## Repository Structure

- **app/galaxy-explorer.ts**  
  The primary script that connects to Coinbase Wallet and queries the Base Sepolia network for relevant data.

- **contracts/**  
  Solidity contracts deployed on Base Sepolia for validation and testing:
  - `control.sol`
  - `arrays.sol`

- **docs/**  
  Documentation to help you understand the usage of Galaxy Explorer:
  - `usage.md`

- **package.json**  
  Contains the project’s dependencies, including libraries for interacting with Coinbase Wallet and Base Sepolia.

- **README.md**  
  This file, which explains the functionality of the project.

---

## Supported Network

Base Sepolia  
chainId (decimal): 84532  
Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

---

## Dependencies

This project relies on the following libraries:
- **Coinbase Wallet SDK**: To connect and interact with Coinbase Wallet
- **Viem**: To interact with the Base Sepolia network
- **Axios**: To make HTTP requests
- **Web3.js**: For extended Ethereum-based interactions
- **Ethers.js**: For interacting with Ethereum protocols

Additionally, this project integrates tools from Base's ecosystem, such as `base-node`, `base-web`, and `coinbase-agentkit`.

---

## License

MIT License  
Copyright (c) 2025 YOUR_NAME

---

## Author contacts

GitHub: [tirades-spare](https://github.com/tirades-spare)  

Email: 0.tirades-spare@icloud.com

Twitter: https://x.com/kochetkovael

---

## Testnet Deployment (Base Sepolia)

These contracts were deployed to Base Sepolia to validate Base Sepolia tooling:

Network: Base Sepolia  
chainId (decimal): 84532  
Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

Contract control.sol address:  
0xDe2C6001D6Ee1a217253ec74f7456088b77AbE65

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0xDe2C6001D6Ee1a217253ec74f7456088b77AbE65)
- [Code Verification](https://sepolia.basescan.org/0xDe2C6001D6Ee1a217253ec74f7456088b77AbE65/0#code)

Contract arrays.sol address:  
0x78b31C8b5Cc04af1b78419B345E6cd4342C2CE3E

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0x78b31C8b5Cc04af1b78419B345E6cd4342C2CE3E)
- [Code Verification](https://sepolia.basescan.org/0x78b31C8b5Cc04af1b78419B345E6cd4342C2CE3E/0#code)

These testnet deployments are used to ensure the functionality of the Base Sepolia network and tooling before launching on Mainnet.
