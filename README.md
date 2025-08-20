# Dex223 Bug Bounty Program

[![Bug Bounty](https://img.shields.io/badge/Bug%20Bounty-Active-brightgreen)](https://github.com/dex223/bug-bounty)
[![Security](https://img.shields.io/badge/Security-Responsible%20Disclosure-blue)](https://github.com/dex223/bug-bounty/blob/main/SECURITY.md)
[![Rewards](https://img.shields.io/badge/Rewards-Up%20to%2030M%20D223-orange)](https://github.com/dex223/bug-bounty/blob/main/REWARDS.md)
[![Status](https://img.shields.io/badge/Status-Active%20Program-success)](https://github.com/dex223/bug-bounty)
[![Community](https://img.shields.io/badge/Community-10%2B%20Security%20Researchers-blueviolet)](https://t.me/Dex223_defi)

## Overview

Welcome to the **Dex223 Bug Bounty Program**! We're committed to maintaining the highest security standards for our decentralized exchange platform built on the ERC-223 token standard. This program encourages security researchers and ethical hackers to identify and responsibly disclose vulnerabilities in our systems.

### About Dex223
Dex223 is a decentralized exchange that addresses the critical security issues of the ERC-20 standard by implementing the ERC-223 token standard. Our platform provides:
- **Enhanced Security**: ERC-223 prevents accidental token loss and removes the need for approvals completely. ERC-223 tokens can be utilized without approve+transferFrom pattern.
- **Backward Compatibility**: Works with existing ERC-20 tokens
- **Encapsulated Margin Trading**: Innovative trading features
- **Fiat Onramp Integration**: On/Off-ramp

## Table of Contents

- [Overview](#overview)
- [Quick Start](#quick-start)
- [How to Submit a Report](#how-to-submit-a-report)
- [Program Scope](#program-scope)
- [Reward Tiers](#reward-tiers)
- [Important Links](#important-links)
- [Contact & Community](#contact--community)

## Quick Start

1. **Read the Rules**: Review our [Program Rules](RULES.md) and [Code of Conduct](CODE_OF_CONDUCT.md)
2. **Set Up Environment**: Follow our [Testing Guide](TESTING_GUIDE.md)
3. **Submit Reports**: Just open a [GitHub issue](https://github.com/rroland10/dex223-bug-bounty/issues) to describe your problem. Our team members will review these public reports and respond in the comments thread.
4. **Get Rewarded**: Check our [Rewards Structure](REWARDS.md)

## How to Submit a Report

**It's super simple!**

1. **Go to**: [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)
2. **Click**: "New Issue"
3. **Choose**: "Bug Report" template
4. **Fill in**: What you found, where it is, how to reproduce it
5. **Submit**: That's it!

**No complex forms, no email templates, no PGP keys - just a simple GitHub issue!**

Our team members will review these public reports and respond in the comments thread.

## Program Scope

### Smart Contract Source Codes
The bug bounty program covers the following smart contract source codes:
- **Repository**: [Dex223-contracts](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/253367297d9093db21661b297cdbb104d8579e35)
- **Focus Areas**: All smart contracts within the defined scope, excluding specific modules listed below

### In Scope
- **Smart Contracts**: All Dex223 smart contracts on Ethereum mainnet and testnets
- **Web Application**: Frontend and backend services at https://test-app.dex223.io
- **API Endpoints**: All public and authenticated APIs including Fiat on/off-ramp integration
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Environment**: https://test-app.dex223.io
- **Infrastructure**: Cloud services and deployment pipelines

### Test Environment
- **Test App**: https://test-app.dex223.io
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Tokens**: Use "Get free tokens" button on test pages
- **Sepolia ETH**: [Chainlink Faucet](https://faucets.chain.link/sepolia) or [Alchemy Faucet](https://www.alchemy.com/faucets/ethereum-sepolia)

### Security Features
- **ERC-223 Standard**: Enhanced token security
- **Multi-Signature Wallets**: Advanced access control
- **Automated Auditing**: Continuous vulnerability scanning
- **Responsible Disclosure**: Coordinated security updates

### Out of Scope
- **Excluded Modules**:
  - **MarginModule**: [Dex223MarginModule.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/253367297d9093db21661b297cdbb104d8579e35/contracts/dex-core/Dex223MarginModule.sol) - Work-in-progress module not ready for security testing
  - **PriceOracle for MarginModule**: [Dex223Oracle.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/253367297d9093db21661b297cdbb104d8579e35/contracts/dex-core/Dex223Oracle.sol) - Oracle implementation specifically designed for the MarginModule
- Social engineering attacks
- Physical security assessments
- Third-party services not under our control
- Known vulnerabilities in dependencies

### Known Issues
The following issues are already known and should not be reported as new vulnerabilities:

1. **Pool Creation Error**: Error in pool creation for a token pair where one token is ERC-20 Original and the other is ERC-223 Original without an existing ERC-20 wrapper.

2. **Auto-conversion Issue**: Auto-conversion of ERC-20 wrapper-tokens to ERC-223 origin in a pair where one token is ERC-20 Origin and the other is ERC-223 Origin does not happen when there is only ERC-20-side liquidity in that pool.

## Reward Tiers

| Severity | Reward | Description |
|----------|---------|-------------|
| **Critical** | 30M D223 | A vulnerability that can completely break the contracts workflow |
| **High** | 7M D223 | A bug report that indicates a high severity problem but can't impact the whole platform |
| **Medium** | 3M D223 | A low-severity problem that can lead to a loss of funds but under specific conditions |
| **Info** | 1M D223 | Anything else - best practices, documentation improvements, etc. |

## Important Links

- [Program Rules](RULES.md)
- [Rewards Structure](REWARDS.md)
- [Security Policy](SECURITY.md)
- [Testing Guide](TESTING_GUIDE.md)
- [Bug Report Template](REPORT_TEMPLATE.md)
- [FAQ](FAQ.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)

## Contact & Community

### Security Contact
- **Primary**: [GitHub Issues](https://github.com/rroland10/dex223-bug-bounty/issues)
- **Telegram**: [Dex223 Channel](https://t.me/Dex223_defi)
- **Discord**: [Dex223 Community](https://discord.gg/t5bdeGC5Jk)

### Social Media & Resources
- **Twitter**: [@Dex_223](https://x.com/Dex_223)
- **YouTube**: [ERC223 Channel](https://www.youtube.com/@erc223)
- **Reddit**: [r/Dex223](https://www.reddit.com/r/Dex223)
- **Medium**: [Dexaran's Blog](https://dexaran820.medium.com/)
- **GitHub**: [EthereumCommonwealth](https://github.com/EthereumCommonwealth)

### Project Resources
- **Latest Development Report**: [July 2025](https://gist.github.com/Dexaran/c479c626a1af52853f5e396d2b7fcf9f)
- **White Paper (Draft)**: [Google Docs](https://docs.google.com/document/d/1Ndz-kqrz4bZV-VwxnmgTW6jz9QsoKgy3zHehcNNGLYM/edit)
- **Pitch Deck**: [DocSend](https://docsend.com/view/zdcya97tgiiiqvwy)
- **Tokenomics**: [Dex223.io](http://dex223.io/#tokenomics)
- **Where to Buy**: [Dex223.io](https://www.dex223.io)
- **Market Data**: [CoinMarketCap](https://coinmarketcap.com/currencies/dex223/)

---

**Important**: Always follow responsible disclosure practices. Do not exploit vulnerabilities beyond what's necessary to demonstrate the issue.

---

*Last updated: July 2025* 