# 🥞 Pancake-Style Prediction (Clone) — Multi-Chain DeFi Market
**Predict. Lock. Win. Across All Chains.** 🌐🔮  

![Banner](A_promotional_digital_graphic_design_banner_showca.png)

---

## 🚀 Overview
This repository contains a **multi-chain PancakeSwap-style Prediction Market** — an open-source platform for building and deploying on-chain UP/DOWN prediction games.

Users predict whether the next price of an asset will be **UP 📈** or **DOWN 📉** in each timed round (default 5 minutes).  
Accurate predictions win rewards from the prize pool, secured and verified by **oracle data** such as **Chainlink**, **Pyth**, or **custom feeds**.

Built for **Ethereum, BNB Chain, Polygon, Arbitrum, Optimism, Avalanche, Base**, and more.

---

## ✨ Highlights
✅ Multi-chain compatible (EVM-based networks)  
✅ 5-minute or configurable round lifecycle (Open → Lock → Close)  
✅ Chainlink / Pyth / custom oracle integration  
✅ Auto round management (Chainlink Keepers, Cron, or script executor)  
✅ Real-time pool tracking and analytics  
✅ Next.js + Tailwind UI for prediction dashboard  
✅ Full REST & WebSocket backend APIs  
✅ Token reward pools, referral bonuses, and leaderboard modules  
✅ Custom themes: Gold, Dark, and Futuristic modes  

---

## 🧩 Architecture
```
Smart Contracts  →  Oracle Feed  →  Backend (Node/TS)  →  Frontend (Next.js/React)
        ↘ Automation / Keeper  ↙
```
**Round Flow**  
1️⃣ Round Opens — users bet UP or DOWN  
2️⃣ Locked — oracle snapshot stored  
3️⃣ Live — market moves, countdown active  
4️⃣ Closed — final oracle price decides winners  
5️⃣ Prize distributed, next round auto-starts  

---

## ⚙️ Tech Stack
**Smart Contracts:** Solidity / Hardhat  
**Backend:** Node.js + TypeScript (Express / Cron Jobs)  
**Frontend:** Next.js + React + Tailwind  
**Database:** MySQL / PostgreSQL  
**Oracles:** Chainlink, Pyth, custom API  
**Automation:** Chainlink Keepers / PM2 Cron / Manual Trigger  

---

## 🛠️ Quick Start

```bash
# 1. Clone repo
git clone https://github.com/yourname/pancake-prediction-clone.git

# 2. Install dependencies
cd contracts && npm install
npx hardhat compile

# 3. Setup environment
cp .env.example .env
# Fill in: RPC_URL, PRIVATE_KEY, ORACLE_FEED, ADMIN_ADDRESS, NETWORK_NAME

# 4. Deploy to any EVM chain
npx hardhat run scripts/deploy.js --network polygon
# or: bsc, ethereum, arbitrum, optimism, avalanche, base

# 5. Start backend indexer
cd backend && npm install && npm run start

# 6. Launch frontend
cd frontend && npm install && npm run dev
```

---

## 🌍 Supported Networks
| Network | Status | Oracle Source |
|----------|---------|----------------|
| BNB Chain | ✅ Stable | Chainlink |
| Ethereum | ✅ Stable | Chainlink / Pyth |
| Polygon | ✅ Stable | Chainlink |
| Arbitrum | 🧪 Beta | Chainlink |
| Avalanche | 🧪 Beta | Chainlink / Pyth |
| Base | 🧪 Beta | Pyth |
| Optimism | 🔧 Experimental | Chainlink |

---

## 🧠 Advanced Features
🧩 Multi-asset pools (BNB, ETH, BTC, Gold, FX pairs)  
🎮 Gamified UI with animations and sound effects  
📊 Live analytics and history tracking  
💰 Referral & commission system  
🪙 Tokenized betting with your own ERC-20 token  
🔄 Dynamic round timers (30s – 15m)  
🧱 Modular backend for Telegram or Discord bot integration  

---

## 🧰 Folder Structure
```
contracts/   →  Solidity smart contracts
backend/     →  Node.js indexer, API, and automation
frontend/    →  Next.js UI dashboard
bots/        →  Optional auto-bet or analytics bots
docs/        →  Setup, API, and deployment guides
```

---

## 📡 API Endpoints (Example)
| Endpoint | Description |
|-----------|-------------|
| `/api/rounds/current` | Get live round info |
| `/api/rounds/history` | Fetch previous rounds |
| `/api/bets/place` | Place a bet (UP/DOWN) |
| `/api/pools` | Get current pool stats |
| `/api/user/:wallet` | Fetch user history |

---

## ⚖️ Security & Legal Notice
> ⚠️ Always audit before deploying to mainnet.  
> ⚠️ Check your region’s laws on prediction or gaming markets.  
> ⚠️ Codemen and contributors are not responsible for misuse or losses.

Recommended:
- Add `Ownable` or `AccessControl` for admin protection  
- Use `reentrancyGuard` and safe math libraries  
- Configure withdrawal & fee caps  

---

## 🪙 Token Integration
Easily integrate your own ERC-20 token for betting and reward payouts.  
Add tokenomics like:
- Burning a % of losing bets  
- Redistributing fees to holders  
- Staking / yield farm tie-ins  

---

## 🖥️ Frontend Demo
The UI is built with **Next.js**, **Tailwind**, and **Framer Motion** for smooth interactions:
- Live price card
- Animated timers
- Responsive Swiper rounds
- Real-time chart (TradingView widget optional)

---

## 🧑‍💻 Developer Contact
📧 **Email:** [codemenco@gmail.com](mailto:codemenco@gmail.com)  
💬 **Telegram:** [+1 205 724 9145](https://t.me/+12057249145)  
🌐 **Website:** [https://codemen.me](https://codemen.me)

---

## 📜 License
Released under the **MIT License**.  
Fork it, modify it, deploy it — attribution appreciated.

---

## 🧭 Credits & Inspiration
Built by **Codemen**  
Inspired by PancakeSwap Prediction, Chainlink Oracles, and the growing DeFi gaming ecosystem.  

![Logo](A_flat_digital_graphic_logo_features_promotional_c.png)

> 🥞 “Predict. Lock. Win.” — now multi-chain.  
> Launch your own on-chain prediction platform today with [codemen.me](https://codemen.me)
