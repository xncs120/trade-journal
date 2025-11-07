# TradeTally `v2.1.2 20250711`
A comprehensive trading journal and analytics platform built with Vue.js frontend and Node.js backend. Track your trades, analyze performance, and gain insights into your trading patterns across multiple brokers.

## Features
### Trading Journal & Analysis
- [x] Multi-Broker Support - Import trades from Lightspeed, Charles Schwab, ThinkorSwim, IBKR, E*TRADE, ProjectX
- [x] Options & Futures Trading - Full support for options and futures contracts with specialized analytics
- [x] Real-time Market Data - Live stock quotes and unrealized P&L tracking
- [x] Trade Visualization - Interactive candlestick charts with entry/exit markers
### Analytics & Insights
- [x] AI-Powered Analytics - Personalized trading recommendations powered by Google Gemini
- [x] Advanced Charts - Performance analysis by hold time, day of week, sector, and more
- [x] Behavioral Analytics - Revenge trading detection and overconfidence tracking (Pro)
- [x] Health Tracking - Correlate sleep, heart rate, and other health metrics with trading performance (Pro)
### Markets & Alerts
- [x] Watchlists - Track favorite stocks with real-time prices and news (Pro)
- [x] Price Alerts - Email and browser notifications for price targets (Pro)
- [x] News Integration - Automatic news enrichment for traded symbols
- [x] Earnings Tracking - Monitor upcoming earnings for watchlist symbols (Pro)
### Community & Gamification
- [x] Leaderboards - Track achievements and compete with peers
- [x] Public Trades - Share trades and learn from the community
- [x] Achievements System - Unlock badges and track milestones
- [x] Forum Integration - Join discussions at [forum.tradetally.io](https://forum.tradetally.io)
### Mobile App
- [x] iOS App - Native iOS application available on [TestFlight](https://testflight.apple.com/join/11shUY3t)
- [x] Full feature parity with web application
- [x] Optimized mobile trading journal experience

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

## Reference and external source
- [TradeTally](https://github.com/GeneBO98/tradetally)