# FreelanceVault 🔐

### Blockchain-Based Freelance Escrow Platform

FreelanceVault is a decentralized freelancing payment platform that uses **blockchain smart contracts to securely hold and release payments between clients and freelancers**.

The goal is to create a simple alternative to traditional freelance payment systems where a smart contract acts as an escrow.

---

## 🚀 Problem

Freelancers working with international clients can face problems such as:

* Payment delays
* Payment disputes
* Lack of trust between clients and freelancers
* High transaction/platform fees
* Unclear milestone-based payments

FreelanceVault aims to solve this by using a **smart contract as a trustless escrow layer**.

---

## 💡 How It Works

```text
Client
   │
   │ Creates Project
   ▼
Smart Contract
   │
   │ Locks Payment
   ▼
Freelancer
   │
   │ Completes Work
   ▼
Client Approves
   │
   ▼
Smart Contract
   │
   │ Releases Payment
   ▼
Freelancer Wallet
```

The smart contract holds the payment until the client approves the completed work.

---

## ✨ MVP Features

### Client

* Connect crypto wallet
* Create a freelance project
* Set project amount
* Deposit payment into escrow
* Review submitted work
* Approve completed work
* Receive refund when applicable

### Freelancer

* Connect wallet
* View available projects
* Accept a project
* Submit completed work
* Receive payment after approval

### Blockchain

* Smart-contract escrow
* Wallet-based authentication
* On-chain transactions
* Payment release through smart contract

---

## 🛠️ Tech Stack

### Frontend

* React
* TypeScript
* Tailwind CSS

### Blockchain

* Solidity
* Ethereum-compatible testnet
* Hardhat
* MetaMask

### Web3

* wagmi
* viem

### Backend

Planned for later:

* Node.js
* Express.js
* MongoDB

---

## 🏗️ Planned Architecture

```text
                    FreelanceVault
                         │
              ┌──────────┴──────────┐
              │                     │
           Client               Freelancer
              │                     │
              └──────────┬──────────┘
                         │
                    React Frontend
                         │
                    wagmi / viem
                         │
                    MetaMask Wallet
                         │
                         ▼
                 FreelanceEscrow.sol
                         │
                         ▼
                 Blockchain Network
```

---

## 📁 Planned Project Structure

```text
freelance-vault/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── contracts/
│   │   └── services/
│   └── package.json
│
├── blockchain/
│   ├── contracts/
│   │   └── FreelanceEscrow.sol
│   ├── scripts/
│   ├── test/
│   └── hardhat.config.js
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   └── server.js
│
├── README.md
└── .gitignore
```

---

## 🔐 Smart Contract

The first version of the smart contract will contain only the essential escrow functions:

```text
createProject()
depositFunds()
submitWork()
approveWork()
releasePayment()
refundClient()
```

The project will initially use **testnet funds only**.

No real-money transactions will be used during development.

---

## 🗺️ Development Roadmap

### Phase 1 — Blockchain Basics

* Learn Solidity fundamentals
* Create the escrow smart contract
* Deploy contract locally
* Write smart-contract tests

### Phase 2 — Testnet

* Deploy contract to an EVM testnet
* Interact with the contract
* Understand transactions, gas and contract state

### Phase 3 — Frontend

* Build React interface
* Connect MetaMask
* Connect frontend to smart contract
* Create client dashboard
* Create freelancer dashboard

### Phase 4 — Escrow Flow

* Create project
* Deposit funds
* Submit work
* Approve work
* Release payment

### Phase 5 — Backend

* Store project metadata
* Store user profiles
* Store transaction references
* Add project history

### Phase 6 — Improvements

* Milestone-based payments
* Dispute mechanism
* Freelancer reputation
* Notifications
* Better UI/UX

---

## 🎯 Learning Goals

This project is being built to understand:

* Blockchain fundamentals
* Solidity
* Smart contracts
* Ethereum transactions
* Wallet integration
* Web3 development
* React + Web3
* Decentralized escrow
* Backend integration
* Full-stack Web3 application development

---

## ⚠️ Disclaimer

This is an educational project and should initially be used only with testnet assets.

It is not intended to handle real financial transactions.

---

## 📌 Project Status

**Status:** 🚧 Initial Setup

Currently working on:

* [x] Project idea
* [x] Architecture
* [x] README
* [ ] Repository setup
* [ ] Solidity environment
* [ ] Escrow smart contract
* [ ] Smart-contract tests
* [ ] Testnet deployment
* [ ] React frontend
* [ ] Wallet integration
* [ ] Full escrow flow

---

## 👩‍💻 Author

**Rajshree Sinha**

B.Tech CSE
Dayananda Sagar University, Bengaluru
