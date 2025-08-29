# GitHub Issue Templates

This directory contains templates to make it easy to submit reports and interact with the Dex223 Bug Bounty Program.

## Available Templates

### Bug Report
Use this template to report security vulnerabilities or bugs you've found.

**What to include:**
- Clear description of the issue
- Where it's located
- How to reproduce it
- Evidence (screenshots, code, etc.)
- Your contact information for rewards

### Feature Request
Use this template to suggest improvements to the bug bounty program.

**What to include:**
- Description of the feature
- Problem it solves
- How it should work
- Any alternatives you've considered

### Question
Use this template to ask questions about the program or get help.

**What to include:**
- Your question
- What you've already tried
- Any relevant context

## How to Use

**It's super simple!**

1. Go to [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)
2. Click "New Issue"
3. Choose the appropriate template
4. Fill in the information
5. Submit the issue

**No complex forms, no email templates, no PGP keys - just a simple GitHub issue!**

## Security Notes

- **Public Issues**: Most issues are public and visible to everyone
- **Sensitive Reports**: For extremely sensitive vulnerabilities, consider using GitHub Security Advisories
- **Responsible Disclosure**: Always follow responsible disclosure practices

## Rewards

Valid security reports are eligible for rewards in D223 tokens:

- **Critical**: 30M D223 - A vulnerability that can completely break the contracts workflow
- **High**: 7M D223 - A bug report that indicates a high severity problem but can't impact the whole platform
- **Medium**: 3M D223 - A low-severity problem that can lead to a loss of funds but under specific conditions
- **Info**: 1M D223 - Anything else - best practices, documentation improvements, etc.

See our [Rewards Structure](../REWARDS.md) for complete details.

## Program Scope

### Smart Contract Source Codes
The bug bounty program covers the following smart contract source codes:
- **Repository**: [Dex223-contracts](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/253367297d9093db21661b297cdbb104d8579e35)
- **Focus Areas**: All smart contracts within the defined scope, excluding specific modules listed below

### In Scope
- **Smart Contracts**: All Dex223 contracts on Ethereum mainnet and testnets
- **Web Application**: Frontend and backend services at https://test-app.dex223.io
- **API Endpoints**: All public and authenticated APIs including Fiat on/off-ramp integration
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Environment**: https://test-app.dex223.io
- **Infrastructure**: Cloud services and deployment pipelines

### Out of Scope
- **Excluded Modules**:
  - **MarginModule**: Work-in-progress module not ready for security testing
  - **PriceOracle for MarginModule**: Oracle implementation specifically designed for the MarginModule
- Social engineering attacks (without permission)
- Physical security assessments
- Third-party services not owned by Dex223
- Known vulnerabilities in dependencies
- Denial of service attacks

### Known Issues
The following issues are already known and should not be reported as new vulnerabilities:

1. **Pool Creation Error**: Error in pool creation for a token pair where one token is ERC-20 Original and the other is ERC-223 Original without an existing ERC-20 wrapper.

2. **Auto-conversion Issue**: Auto-conversion of ERC-20 wrapper-tokens to ERC-223 origin in a pair where one token is ERC-20 Origin and the other is ERC-223 Origin does not happen when there is only ERC-20-side liquidity in that pool.

### Test Environment Access
- **Test App**: https://test-app.dex223.io
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Tokens**: Use "Get free tokens" button on test pages
- **Sepolia ETH**: Available through [Chainlink](https://faucets.chain.link/sepolia) and [Alchemy](https://www.alchemy.com/faucets/ethereum-sepolia) faucets

---

**Need help?** Join our [Telegram](https://t.me/Dex223_defi) or [Discord](https://discord.gg/t5bdeGC5Jk) community!

*Last Updated: July 2025*
