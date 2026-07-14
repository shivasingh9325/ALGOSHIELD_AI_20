

# 🛡️ AlgoShield AI

### AI-Powered Smart Contract Security Platform for the Algorand Blockchain

<p align="center">

![Algorand](https://img.shields.io/badge/Algorand-000?style=for-the-badge\&logo=algorand)
![AI Powered](https://img.shields.io/badge/AI--Powered-00C853?style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge\&logo=fastapi)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python)
![MIT License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</p>

---

## 🚀 Overview

**AlgoShield AI** is an AI-powered smart contract security platform built for the **Algorand Blockchain**.

The platform helps developers identify vulnerabilities before deployment, receive AI-generated remediation suggestions, continuously monitor deployed contracts, and certify secure contracts through NFT-based security certificates.

Instead of relying on expensive manual audits, AlgoShield AI automates the complete smart contract security lifecycle using Machine Learning, Retrieval-Augmented Generation (RAG), Small Language Models (SLMs), and real-time blockchain monitoring.

---

# ❓ The Problem

Smart contracts are immutable.

A single vulnerability can permanently lock funds, expose critical exploits, or lead to millions of dollars in losses.

Most developers face challenges such as:

* Expensive manual security audits
* Lack of real-time monitoring
* No automated vulnerability detection
* Generic AI suggestions
* No security certification mechanism

Security often becomes the bottleneck during deployment.

---

# 💡 Our Solution

AlgoShield AI provides an end-to-end security ecosystem that assists developers throughout the complete lifecycle of a smart contract.

It enables developers to:

* Scan contracts using Machine Learning
* Detect known vulnerabilities
* Generate AI-powered code fixes
* Monitor deployed contracts 24/7
* Receive Email & Telegram alerts
* Mint blockchain-based security certificates
* Integrate security checks into CI/CD pipelines

---

# ✨ Features

| Feature                       | Description                                                          |
| ----------------------------- | -------------------------------------------------------------------- |
| 🔍 AI Vulnerability Scanner   | Detects risky TEAL contracts using ML models and rule-based analysis |
| 🧠 AI Code Suggestions        | Uses RAG + Phi-3 Mini SLM to generate intelligent code fixes         |
| 📊 Security Dashboard         | Beautiful React dashboard with real-time reports                     |
| 📡 Live Blockchain Monitoring | Monitors deployed smart contracts continuously                       |
| 📧 Email Alerts               | Instant HTML email notifications                                     |
| 📱 Telegram Alerts            | Receive critical alerts directly on Telegram                         |
| 🏆 NFT Security Certificate   | Mint ARC-69 certificates for secure contracts                        |
| ⚡ CLI & SDK                   | Scan contracts directly from terminal or CI/CD                       |
| 📈 Risk Score                 | Confidence-based Safe/Risky classification                           |
| 🔄 Watch Mode                 | Continuously scans contracts while developing                        |

---

# 🏗 System Architecture

```text
                         +---------------------------+
                         |       React Frontend      |
                         |  Dashboard • Scanner      |
                         | Certificates • Monitor    |
                         +------------+--------------+
                                      |
                                   REST API
                                      |
                +---------------------+----------------------+
                |                                            |
        +-------v-------+                          +----------v---------+
        | FastAPI API   |                          | Monitoring Service |
        |---------------|                          | APScheduler        |
        | ML Scanner    |                          | Indexer Polling    |
        | Rule Engine   |                          | Alerts             |
        | RAG Pipeline  |                          +----------+---------+
        | NFT Minting   |                                     |
        +-------+-------+                                     |
                |                                             |
     +----------+----------+                     +-------------+-----------+
     |                     |                     |                         |
+----v----+         +------v------+       +------v------+          +------v------+
| MongoDB |         | ChromaDB    |       | Supabase    |          | Algorand    |
| Scans   |         | Vector DB   |       | Monitoring  |          | Blockchain  |
+---------+         +-------------+       +-------------+          +-------------+
```

---

# 🧠 AI Pipeline

```
Contract
      │
      ▼

Feature Extraction

      │
      ▼

Random Forest Classifier

      │
      ▼

Rule Based Engine

      │
      ▼

Risk Score Generation

      │
      ▼

RAG Retrieval

      │
      ▼

Phi-3 Mini SLM

      │
      ▼

AI Generated Fix Suggestions
```

---

# 🛠 Tech Stack

## Frontend

* React
* TypeScript
* Vite
* Tailwind CSS
* Framer Motion
* Three.js
* Pera Wallet

---

## Backend

* FastAPI
* Python
* APScheduler
* Motor
* JWT Authentication

---

## AI / ML

* Scikit-learn
* Random Forest
* Isolation Forest
* ChromaDB
* llama-cpp-python
* Phi-3 Mini
* RAG Pipeline

---

## Blockchain

* Algorand SDK
* ARC-69 NFT Standard
* Algonode Indexer
* Pera Wallet

---

## Database

* MongoDB
* Supabase

---

# 📂 Project Structure

```text
AlgoShield_AI/

projects/

├── backend/
│   ├── blockchain/
│   ├── routes/
│   ├── services/
│   ├── ml_models/
│   ├── utils/
│   └── app.py
│
├── frontend/
│
├── frontend-jsx/
│
├── algoshield-sdk/
│
├── contracts/
│
├── dataset/
│
├── docs/
│
└── README.md
```

---

# ⚙ Installation

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/AlgoShield_AI.git

cd AlgoShield_AI
```

---

## Backend

```bash
cd projects/backend

python -m venv venv

# Windows

venv\Scripts\activate

# Linux/Mac

source venv/bin/activate

pip install -r requirements.txt

python app.py
```

---

## Frontend

```bash
cd projects/frontend

npm install

npm run dev
```

---

## SDK

```bash
cd projects/algoshield-sdk

npm install

node bin/algoshield.js
```

---

# 🔑 Environment Variables

Create a `.env` file inside the backend folder.

```env
MONGODB_URL=

MONGODB_DB_NAME=

SUPABASE_URL=

SUPABASE_KEY=

PLATFORM_MNEMONIC=

INDEXER_API_URL=

SMTP_USER=

SMTP_PASSWORD=

SMTP_HOST=

SMTP_PORT=

ALERT_FROM_EMAIL=

TELEGRAM_BOT_TOKEN=

TELEGRAM_CHAT_ID=
```

---

# 📡 REST API

| Method | Endpoint             | Description          |
| ------ | -------------------- | -------------------- |
| POST   | `/api/scan`          | Scan Smart Contract  |
| GET    | `/api/scan/{id}`     | Fetch Scan Report    |
| POST   | `/api/monitor`       | Register Monitoring  |
| DELETE | `/api/monitor/{id}`  | Remove Monitoring    |
| POST   | `/api/mint/{scanId}` | Mint NFT Certificate |

---

# 🎬 Demo Workflow

### Connect Wallet

Connect your Pera Wallet.

↓

### Upload Contract

Upload a TEAL contract.

↓

### AI Scan

The ML engine analyzes vulnerabilities.

↓

### AI Suggestions

Generate intelligent fixes using RAG.

↓

### Security Report

Receive confidence score and risk level.

↓

### NFT Certificate

Mint ARC-69 Security NFT if score ≥ 70.

↓

### Live Monitoring

Monitor deployed contracts 24/7.

↓

### Email & Telegram Alerts

Receive notifications whenever suspicious activity is detected.

---

# 📊 Security Workflow

```
Write Contract

↓

Upload Contract

↓

ML Analysis

↓

Rule Validation

↓

AI Suggestions

↓

Deploy

↓

Continuous Monitoring

↓

Alerts

↓

Security Certificate
```

---

# 🚀 Future Roadmap

* Smart Contract Auto-Patching
* VS Code Extension
* GitHub Actions Integration
* Multi-chain Support
* AI Threat Prediction
* Developer Analytics Dashboard
* Security Leaderboard
* Audit History Timeline

---

# 🤝 Team

Developed with ❤️ by **Team QANTAS**

Built for the **Algorand 3.0 Hack Series**

---

# 📜 License

This project is licensed under the **MIT License**.

---

# ⭐ Support

If you found this project useful,

⭐ Star this repository

🍴 Fork it

🤝 Contribute

💬 Share your feedback

---

> **"Secure Smart Contracts. Build with Confidence."**
>
> **AlgoShield AI**
