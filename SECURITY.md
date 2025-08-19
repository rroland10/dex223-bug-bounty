# Dex223 Security Policy

## Responsible Disclosure

Dex223 is committed to maintaining the highest security standards through proactive vulnerability management and collaborative security research. We believe that working with the global security community is crucial to identifying and fixing vulnerabilities before they can be exploited maliciously. As a decentralized team, we value community-driven approaches and flexibility.

### Disclosure Timeline

We aim to address vulnerabilities as quickly as possible:
- **Initial Response**: Within 1-7 days for acknowledgment
- **Assessment**: 1-4 weeks for vulnerability assessment and fix development
- **Deployment**: 2-8 weeks for fix deployment and testing
- **Public Disclosure**: Coordinated disclosure when fixes are ready

*Note: Timeline may vary based on complexity and team availability*

### Security Contact

- **Primary**: [GitHub Issues](https://github.com/rroland10/dex223-bug-bounty/issues)
- **Telegram**: [Dex223 Security Channel](https://t.me/Dex223_defi)
- **Discord**: [Dex223 Community](https://discord.gg/t5bdeGC5Jk)
- **GitHub**: [EthereumCommonwealth](https://github.com/EthereumCommonwealth)
- **Emergency**: Telegram security channel

### Reporting Guidelines

**It's super simple!**

1. **Go to**: [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)
2. **Click**: "New Issue"
3. **Choose**: "Bug Report" template
4. **Fill in**: What you found, where it is, how to reproduce it
5. **Submit**: That's it!

**No complex forms, no email templates, no PGP keys - just a simple GitHub issue!**

### What Not to Do

- **Don't exploit** vulnerabilities beyond proof of concept
- **Don't access** other users' data without permission
- **Don't perform** denial of service attacks
- **Don't publicly disclose** before coordination
- **Don't attempt** social engineering without approval

### What We Promise

- **Response** to all reports when possible
- **Fair assessment** of vulnerability severity
- **Appropriate rewards** in D223 tokens for valid findings
- **Public acknowledgment** of researchers
- **No legal action** for good-faith testing

## Reward Structure

### D223 Token Rewards
We reward security researchers with our native D223 tokens:

- **Critical**: 30M D223 - A vulnerability that can completely break the contracts workflow
- **High**: 7M D223 - A bug report that indicates a high severity problem but can't impact the whole platform
- **Medium**: 3M D223 - A low-severity problem that can lead to a loss of funds but under specific conditions
- **Info**: 1M D223 - Anything else - best practices, documentation improvements, etc.

### Payment Process
- **Rewards paid in D223 tokens only**
- **Payment timeline**: 1-12 weeks depending on severity
- **Wallet verification** required before payment


## Security Scope

### In Scope
- **Smart Contracts**: All Dex223 contracts on Ethereum mainnet and testnets
- **Web Application**: Frontend and backend services at https://test-app.dex223.io
- **API Endpoints**: All public and authenticated APIs including Fiat on/off-ramp integration
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Environment**: https://test-app.dex223.io
- **Infrastructure**: Cloud services and deployment pipelines

### Out of Scope
- Social engineering attacks (without permission)
- Physical security assessments
- Third-party services not owned by Dex223
- Known vulnerabilities in dependencies
- Denial of service attacks

## Testing Guidelines

### Safe Testing Practices
- **Use test environment** when possible
- **Follow responsible disclosure** timeline
- **Document findings** thoroughly
- **Coordinate critical issues** immediately
- **Respect rate limits** and testing boundaries

### Test Environment Access
- **Test App**: https://test-app.dex223.io
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Tokens**: Use "Get free tokens" button on test pages
- **Sepolia ETH**: Available through Chainlink and Alchemy faucets

---

**Last Updated**: July 2025 