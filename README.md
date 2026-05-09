# 🔗 KiiChain Micro Lending dApp

> **Week 2 — KiiChain Builder Series**
> A beginner-friendly decentralized micro lending smart contract built on KiiChain Testnet Oro.

![KiiChain](https://img.shields.io/badge/KiiChain-Testnet%20Oro-7c3aed?style=for-the-badge)
![Chain ID](https://img.shields.io/badge/Chain%20ID-1336-a855f7?style=for-the-badge)
![ethers.js](https://img.shields.io/badge/ethers.js-5.7-22d3ee?style=for-the-badge)
![Live](https://img.shields.io/badge/Status-Live-4ade80?style=for-the-badge)

---

## ✨ Features

| Feature | Description |
|---|---|
| 💜 Deposit KII | Deposit native KII tokens to the smart contract |
| 🤝 Request Loan | Borrow KII from protocol liquidity |
| 🔄 Repay Loan | Repay your active loan in full |
| 📊 Live Balances | Real-time onchain data reads |
| 🦊 MetaMask | Full wallet connection & network switching |
| 🔔 Notifications | Toast alerts for every TX state |
| 📜 TX History | Session transaction history with explorer links |

---

## 🚀 Live Demo

> Deployed on Vercel — https://kiichain-microlending.vercel.app/

---

## 🧱 Tech Stack

- **Frontend** — Pure HTML/CSS/JS (single file, no build step)
- **Web3** — [ethers.js v5](https://docs.ethers.io/v5/) via CDN
- **Wallet** — MetaMask (EIP-1193 provider)
- **Blockchain** — KiiChain Testnet Oro (EVM-compatible)
- **Hosting** — Vercel (static deployment)

---

## 📋 Smart Contract

| Field | Value |
|---|---|
| **Address** | `0x3c0Bfc4f12703074dD013bE7555F9fC49cA462F7` |
| **Network** | KiiChain Testnet Oro |
| **Chain ID** | `1336` |
| **Currency** | `KII` |
| **RPC** | `https://json-rpc.uno.sentry.testnet.v3.kiivalidator.com/` |
| **Explorer** | [testnet.explorer.kiichain.io](https://testnet.explorer.kiichain.io/) |

### Contract Functions

```solidity
// Deposit KII into the contract
function deposit() external payable

// Request a loan (amount in wei)
function requestLoan(uint256 amount) external

// Repay active loan (send exact loan amount)
function repayLoan() external payable

// Read deposit balance of a user
function getDeposit(address user) external view returns (uint256)

// Read active loan of a user
function getLoan(address user) external view returns (uint256)
```

---

## 🛠 Local Development

No build step required. Simply open `index.html` in a browser with MetaMask installed:

```bash
# Clone the repo
git clone https://github.com/Kbin1992/kiichain-microlending-dapp.git
cd kiichain-microlending-dapp

# Open directly (macOS)
open index.html

# Or use a local dev server
npx serve .
```

---

## 🌐 Deploy to Vercel

### Option 1 — Vercel CLI

```bash
npm i -g vercel
vercel
```

### Option 2 — GitHub Integration

1. Push this repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import your GitHub repository
4. Vercel auto-detects static HTML — click **Deploy**
5. Done ✅

---

## 🔧 MetaMask Setup

Add KiiChain Testnet Oro manually if needed:

| Field | Value |
|---|---|
| Network Name | KiiChain Testnet Oro |
| RPC URL | `https://json-rpc.uno.sentry.testnet.v3.kiivalidator.com/` |
| Chain ID | `1336` |
| Currency Symbol | `KII` |
| Block Explorer | `https://testnet.explorer.kiichain.io/` |

> 💡 The dApp will auto-prompt MetaMask to add & switch to KiiChain when you click **Connect Wallet**.

---

## 💧 Get Test KII

Visit the [KiiChain Faucet](https://explorer.kiichain.io/faucet) to receive free testnet KII tokens.

---

## 📁 Project Structure

```
kiichain-microlending/
├── index.html        ← Full dApp (Web3 + UI in one file)
├── vercel.json       ← Vercel deployment config
├── .gitignore        ← Standard gitignore
└── README.md         ← This file
```

---

## 🏗 About This Project

This is a **Week 2 KiiChain Builder Series** project exploring decentralized lending mechanics and PayFi infrastructure. The MicroLending smart contract demonstrates how permissionless finance works at a protocol level — anyone can deposit collateral, request loans, and repay without intermediaries.

Built on **KiiChain Testnet Oro**, this project showcases KiiChain's capabilities for real-world financial use cases. KiiChain is purpose-built for PayFi — bridging traditional finance and decentralized infrastructure.

---

## 🔗 Links

- [KiiChain Website](https://kiichain.io)
- [KiiChain Block Explorer](https://testnet.explorer.kiichain.io/)
- [KiiChain Faucet](https://explorer.kiichain.io/faucet)
- [GitHub — Weekly Contracts](https://github.com/Kbin1992/kiichain-weekly-contracts)

---

## 👤 Author

**Built by Kbin** on KiiChain Testnet Oro · Week 2 Builder Series

---

*This project is for educational purposes on KiiChain Testnet. Do not use real funds.*
