# 🏛️ Web3 Smart Tender System

A **blockchain-based transparent tendering platform** that eliminates corruption in government tenders using Ethereum smart contracts, commit-reveal bidding, and AI-powered contractor evaluation.

---

## ✨ Features

- 🔗 **Blockchain-Powered** — All tenders and bids stored immutably on Ethereum
- 🔒 **Commit-Reveal Bidding** — Sealed bids prevent bid manipulation and front-running
- 🤖 **AI Competence Scoring** — Contractors evaluated with AI-generated competence scores
- 👛 **Wallet Authentication** — Login via MetaMask using RainbowKit
- 🏗️ **Milestone Tracking** — Track project milestones with IPFS proof uploads
- 💰 **Auto Payments** — Smart contract automatically releases payments on milestone approval
- 👨‍💼 **Role-Based Access** — Separate portals for Government Officials and Contractors
- 📊 **Transparent Evaluation** — Winner selected using weighted formula (70% price + 30% competence)

---

## 🛠️ Tech Stack

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=black)

### Blockchain
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=ethereum&logoColor=white)
![Wagmi](https://img.shields.io/badge/Wagmi-1C1B1F?style=for-the-badge&logo=ethereum&logoColor=white)
![RainbowKit](https://img.shields.io/badge/RainbowKit-7B3FE4?style=for-the-badge&logo=ethereum&logoColor=white)

---

## 🏗️ Architecture

```
┌─────────────────────────────┐
│        React Frontend       │
│  (Vite + TailwindCSS + GSAP) │
├─────────────────────────────┤
│    Wagmi + RainbowKit       │
│    (Wallet Connection)      │
├─────────────────────────────┤
│   TransparentTender.sol     │
│   (Ethereum Smart Contract) │
├─────────────────────────────┤
│   Ethereum Blockchain       │
└─────────────────────────────┘
```

---

## 📁 Project Structure

```
Web3-Smart-Tender-System/
├── SmartContract/
│   └── TenderContract.sol    # Solidity smart contract
├── src/
│   ├── components/
│   │   └── Navbar.jsx
│   ├── pages/
│   │   ├── Home.jsx              # Landing page
│   │   ├── GovernmentLogin.jsx   # Government official portal
│   │   ├── TenderLogin.jsx       # Tender management portal
│   │   ├── ContractorDashboard.jsx
│   │   ├── AdminDashboard.jsx
│   │   ├── TenderDetails.jsx
│   │   ├── Register.jsx
│   │   └── Signup.jsx
│   ├── abi.json              # Contract ABI
│   ├── wagmi.js              # Wagmi configuration
│   ├── App.jsx
│   └── main.jsx
├── package.json
└── vite.config.js
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- MetaMask browser extension

### Installation

```bash
# Clone the repository
git clone https://github.com/DEVRAJ-20/Web3-Smart-Tender-System.git
cd Web3-Smart-Tender-System

# Install dependencies
npm install

# Start development server
npm run dev
```

The app will be available at `http://localhost:5173`

---

## 📜 Smart Contract

The `TransparentTender.sol` contract handles:

| Module | Description |
|--------|-------------|
| **Access Control** | Government official role management |
| **Contractor Registry** | Registration with IPFS profiles & AI scores |
| **Tender Creation** | Create tenders with commit/reveal deadlines |
| **Commit-Reveal Bidding** | Sealed bid submission and verification |
| **Winner Selection** | Weighted scoring: `(Price × 70) + ((100 - Competence) × 30)` |
| **Milestone Payments** | Track milestones, upload IPFS proofs, auto-pay on approval |

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

**Made by [Devraj K Chandani](https://github.com/DEVRAJ-20)**

</div>
