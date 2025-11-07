# TradeTally `v2.1.2`
A comprehensive trading journal and analytics platform built with Vue.js frontend and Node.js backend. Track your trades, analyze performance, and gain insights into your trading patterns across multiple brokers.

- Cloned from [TradeTally](https://github.com/GeneBO98/tradetally) on 20250711. Please use original instead of this modified version, this version is not maintained.

## Features
### Trading Journal & Analysis
- [x] Multi-Broker Support - Import trades from Lightspeed, Charles Schwab, ThinkorSwim, IBKR, E*TRADE, ProjectX
- [x] Options & Futures Trading - Full support for options and futures contracts with specialized analytics
- [x] Real-time Market Data - Live stock quotes and unrealized P&L tracking
- [x] Trade Visualization - Interactive candlestick charts with entry/exit markers

## Getting started
```sh
git clone this_repo
cd this_repo
cp .env.example .env
// minor change on .env variables
// - DB_USER, DB_PASSWORD, DB_NAME, JWT_SECRET, FRONTEND_URL=http://localhost:3001
// minor change on docker-compose.yaml
// - adminer module: comment whole
// - app module: port "3001:80" (preferred)
docker-compose up -d
// connect to postgres db using any software
// - find migrations table add row 095_create_backup_system.sql to skip this migration (has error)
// access into app docker shell
cd backend
npm run migrate
```