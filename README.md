# 🛡️ SuiShield

**AI-powered smart contract & DeFi risk scanner with Walrus audit trail — built on Sui**

> Sui Overflow 2025 Hackathon Submission | Track: DeFi + AI + Infrastructure

---

## 🎯 What is SuiShield?

SuiShield is an AI-native security intelligence platform for the Sui ecosystem. Developers and DeFi users can scan Move smart contracts or live protocols for vulnerabilities and economic risks — and store every audit report permanently on **Walrus** for on-chain verifiability.

**One line:** *Paste your contract → get an AI risk report → store the proof on Walrus.*

---

## 🧩 The Problem

The Sui DeFi ecosystem is growing fast. But security tooling hasn't kept up:

- Formal audits cost $20K–$100K and take weeks
- There's no public, verifiable audit registry for Sui protocols
- Individual developers can't afford pre-deployment security review
- DeFi risk changes daily — static audits become outdated instantly

---

## ✨ Solution

SuiShield provides three integrated capabilities:

### 1. 🤖 AI Contract Scanner
- Paste any Move smart contract
- AI analyzes for: reentrancy, flash loan exploits, oracle manipulation, access control flaws, arithmetic overflows, lock duration bypass, royalty bypass, and more
- Returns a scored risk report with severity-graded findings

### 2. 📊 DeFi Live Monitor
- Select any Sui DeFi protocol (Haedal, Cetus, Scallop, Turbos...)
- Get real-time risk exposure analysis: depeg risk, liquidity concentration, oracle freshness, collateral health
- Designed to catch risks that static audits miss

### 3. 🐋 Walrus Audit Trail
- Every report is stored as a blob on **Walrus** (Sui's decentralized storage layer)
- The blob ID is registered on Sui — tamper-proof, content-addressed, permanent
- Anyone can retrieve and verify the exact audit that was generated
- Creates an open, public security history for all Sui DeFi

---

## 🏗️ Architecture

```
Move Contract / Protocol Address
        ↓
  Claude AI Engine
  (static analysis + economic logic review)
        ↓
   Risk Report (JSON)
        ↓
  Walrus Blob Storage
  (immutable, content-addressed)
        ↓
  Sui On-chain Blob ID Registration
  (verifiable proof of audit)
```

### Tech Stack

| Layer | Technology |
|-------|-----------|
| Blockchain | Sui Network |
| Storage | Walrus (decentralized blob storage) |
| AI Engine | Claude (Anthropic) |
| Contract Language | Move |
| Frontend | React / Vanilla JS |

---

## 🚀 Why This Matters for Sui

- **DeFi track**: Directly protects and strengthens Sui's DeFi ecosystem
- **AI track**: Uses AI to democratize security review that currently only large protocols can afford
- **Walrus track**: Creates a novel use case for Walrus as a public audit registry — not just file storage

This is infrastructure that benefits every builder in the Sui ecosystem.

---

## 💰 Prize Pool Context

| Award | Amount |
|-------|--------|
| 🥇 1st Place | $800 |
| 🥈 2nd Place | $500 |
| 🥉 3rd Place | $200 |
| 🏅 Demo Session Pool | $500 shared |

---

## 📋 Sui Overflow Evaluation Criteria Alignment

| Criterion | How SuiShield Addresses It |
|-----------|---------------------------|
| **Innovation** | First AI + Walrus audit registry on Sui |
| **Technical Execution** | Working demo with Move contract analysis |
| **Sui Ecosystem Impact** | Security layer for all DeFi protocols |
| **Feasibility** | Deployable with existing Sui + Walrus APIs |
| **Presentation** | Live scanner demo with real Move code |

---

## 🔮 Roadmap

**v0.1 (this hackathon):** Web-based scanner, simulated AI analysis, Walrus storage UI

**v0.2:** Real Claude API integration, live Walrus blob storage via `walrus-ts` SDK

**v0.3:** Sui on-chain registry contract — stores blob IDs + protocol addresses + timestamps

**v1.0:** CI/CD plugin — auto-scan every Move contract on deploy, block deployment if HIGH risk detected

---

## 👤 Builder

Built at **Sui Overflow Taiwan Hacker House**, Taipei — May 2025

Organized by: Bermu DAO × XueDAO × First Movers TW

---

## 📄 License

MIT
