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
- **Repository**: [Dex223-contracts](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/18fa3272c820df349551881d46fb9b13a2bcba62)
- **Focus Areas**: All smart contracts within the defined scope, excluding specific modules listed below

### Deployed Contracts (what to test)
Reports must reproduce against the contracts deployed at these addresses. Each address links to Etherscan. The core and periphery contracts were deployed on October 7, 2026. Every contract in these tables except the token converter matches commit [`18fa327`](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/18fa3272c820df349551881d46fb9b13a2bcba62) byte for byte. You can confirm this with `scripts/check-deployment-hashes.ts` in that repository. The MarginModule and its Oracle were redeployed on October 10, 2026 and also match this commit, but they stay out of scope (see below).

**Ethereum mainnet**

| Contract | Address |
|---|---|
| Factory | [`0x899097B427cd04e1BD07FD3445cc90493300C3a5`](https://etherscan.io/address/0x899097B427cd04e1BD07FD3445cc90493300C3a5#code) |
| Swap router | [`0x14248d524850B0B47B30F4332279330Cad2846a2`](https://etherscan.io/address/0x14248d524850B0B47B30F4332279330Cad2846a2#code) |
| Position manager | [`0x15E22548C572C8Fdb3AcC600c040D5F2A19855D4`](https://etherscan.io/address/0x15E22548C572C8Fdb3AcC600c040D5F2A19855D4#code) |
| Quoter | [`0x69ee81C767cA94e71DDc356D433B30f6eBf7b41E`](https://etherscan.io/address/0x69ee81C767cA94e71DDc356D433B30f6eBf7b41E#code) |
| Core autolisting | [`0x63054Fa5899Bce903E676CC478811bF1fed20E5b`](https://etherscan.io/address/0x63054Fa5899Bce903E676CC478811bF1fed20E5b#code) |
| Free autolisting | [`0xB442f1362163b168cebAd877067D35Eb8d9176d9`](https://etherscan.io/address/0xB442f1362163b168cebAd877067D35Eb8d9176d9#code) |
| Token converter (ERC-7417) | [`0xe7E969012557f25bECddB717A3aa2f4789ba9f9a`](https://etherscan.io/address/0xe7E969012557f25bECddB717A3aa2f4789ba9f9a#code) |

The converter is the original ERC-7417 deployment from March 2025; later converter changes in the repository are not deployed.

**Sepolia (used by https://test-app.dex223.io)**

| Contract | Address |
|---|---|
| Factory | [`0xf07cc56E969Bc08395E80Da099e44d122bFa42B9`](https://sepolia.etherscan.io/address/0xf07cc56E969Bc08395E80Da099e44d122bFa42B9#code) |
| Swap router | [`0x322D53bda812099287BB74baA487c069C5F7B2b1`](https://sepolia.etherscan.io/address/0x322D53bda812099287BB74baA487c069C5F7B2b1#code) |
| Position manager | [`0x1b14B1136BE241565eDa7eB465919C7413a1bb47`](https://sepolia.etherscan.io/address/0x1b14B1136BE241565eDa7eB465919C7413a1bb47#code) |
| Quoter | [`0x11E200C04681e8348beF96c8C1dcfdECFC2dEc0C`](https://sepolia.etherscan.io/address/0x11E200C04681e8348beF96c8C1dcfdECFC2dEc0C#code) |
| Core autolisting | [`0xF35AB968Eb874A56244e7df1D569F06aEf327936`](https://sepolia.etherscan.io/address/0xF35AB968Eb874A56244e7df1D569F06aEf327936#code) |
| Free autolisting | [`0x0F81b549eE7DB363fbbb4358B9004C2AB97C7118`](https://sepolia.etherscan.io/address/0x0F81b549eE7DB363fbbb4358B9004C2AB97C7118#code) |
| Token converter (ERC-7417) | [`0x5847f5C0E09182d9e75fE8B1617786F62fee0D9F`](https://sepolia.etherscan.io/address/0x5847f5C0E09182d9e75fE8B1617786F62fee0D9F#code) |

### Deprecated Deployments
These older contracts are still on-chain but no longer used by the Dex223 app. They are out of scope, except for findings that put funds or token approvals they still hold at risk today.

| Contract | Address |
|---|---|
| Swap router (v1) | [`0xbeBAB9Ab58f8099fbFEb15E14b663615D19304Fa`](https://etherscan.io/address/0xbeBAB9Ab58f8099fbFEb15E14b663615D19304Fa#code) |
| Swap router | [`0x09127e22961C61c2b252b23ff97e6D4689AC13A9`](https://etherscan.io/address/0x09127e22961C61c2b252b23ff97e6D4689AC13A9#code) |
| Swap router | [`0x8702E7647f689D07fdF2827978a19F5fdc662ef8`](https://etherscan.io/address/0x8702E7647f689D07fdF2827978a19F5fdc662ef8#code) |
| Factory (v1) | [`0x8dae173016f65F61e90631Ee5f28C9E47b1ebc06`](https://etherscan.io/address/0x8dae173016f65F61e90631Ee5f28C9E47b1ebc06#code) |
| Factory | [`0xc0c5511f23a268f041Ad10466a17b719942a8F1f`](https://etherscan.io/address/0xc0c5511f23a268f041Ad10466a17b719942a8F1f#code) |

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
  - **MarginModule**: [Dex223MarginModule.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/18fa3272c820df349551881d46fb9b13a2bcba62/contracts/dex-core/Dex223MarginModule.sol) - Work-in-progress module not ready for security testing
  - **PriceOracle for MarginModule**: [Dex223Oracle.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/18fa3272c820df349551881d46fb9b13a2bcba62/contracts/dex-core/Dex223Oracle.sol) - Oracle implementation specifically designed for the MarginModule
- Social engineering attacks
- Physical security assessments
- Third-party services not under our control
- Known vulnerabilities in dependencies

### Known Issues
The following issues are already known and should not be reported as new vulnerabilities:

1. **Pool Creation Error**: Error in pool creation for a token pair where one token is ERC-20 Original and the other is ERC-223 Original without an existing ERC-20 wrapper.

2. **Auto-conversion Issue**: Auto-conversion of ERC-20 wrapper-tokens to ERC-223 origin in a pair where one token is ERC-20 Origin and the other is ERC-223 Origin does not happen when there is only ERC-20-side liquidity in that pool.

3. **Non-standard tokens (fee-on-transfer, rebasing and similar)**: The Token Converter (EIP-7417) and the DEX support only standard ERC-20 and ERC-223 tokens, which deliver exactly the amount they report. Tokens that charge a fee on transfer, rebase, or otherwise deliver a different amount than they report are not supported. Wrappers minted for such a token can end up under-backed, but the effect is confined to holders of that token's own wrapper, because every wrapper is bound to its origin token. Reports whose impact depends on a non-standard token, including calling `tokenReceived` from a contract that is not a real ERC-223 token, are not eligible (see [issue #13](https://github.com/rroland10/dex223-bug-bounty/issues/13)).

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