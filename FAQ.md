# Dex223 Bug Bounty FAQ

## General Questions

### What is the Dex223 Bug Bounty Program?
The Dex223 Bug Bounty Program is a security initiative that rewards researchers for finding and responsibly disclosing vulnerabilities in our decentralized exchange platform. We believe that working with the security community is essential for maintaining the highest security standards.

### Who can participate?
Anyone can participate except:
- Dex223 employees and contractors
- Minors under 18 years old
- Anyone involved in developing the reported vulnerability

### How much can I earn?
Rewards are paid in D223 tokens:
- **Critical**: 30M D223 - A vulnerability that can completely break the contracts workflow
- **High**: 7M D223 - A bug report that indicates a high severity problem but can't impact the whole platform
- **Medium**: 3M D223 - A low-severity problem that can lead to a loss of funds but under specific conditions
- **Info**: 1M D223 - Anything else - best practices, documentation improvements, etc.

*Updated: July 2025*

## Scope Questions

### What's in scope?
- **Smart Contracts**: [Dex223-contracts repository](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/253367297d9093db21661b297cdbb104d8579e35) on Ethereum mainnet and testnets
- **Web Application**: Frontend and backend services at https://test-app.dex223.io
- **API Endpoints**: All public and authenticated APIs including Fiat on/off-ramp integration
- **Swap Interface**: https://test-app.dex223.io/en/swap
- **Test Environment**: https://test-app.dex223.io
- **Infrastructure**: Cloud services and deployment pipelines

### What's out of scope?
- **Excluded Modules**:
  - **MarginModule**: Work-in-progress module not ready for security testing
  - **PriceOracle for MarginModule**: Oracle implementation specifically designed for the MarginModule
- Social engineering attacks (without permission)
- Physical security assessments
- Third-party services not owned by Dex223
- Known vulnerabilities in dependencies
- Denial of service attacks
- Known issues documented in scope (pool creation errors, auto-conversion issues)

### Can I test production systems?
Limited testing is allowed on production systems, but we encourage using our staging environment and testnets. Always follow responsible disclosure practices and don't cause any damage.

## Payment Questions

### How do I get paid?
We pay rewards in **D223 tokens only**:
- **Primary**: D223 tokens (our native cryptocurrency)
- **Distribution**: Tokens are sent to your provided wallet address
- **Verification**: We verify your wallet address before payment

### When do I get paid?
We aim to process payments as quickly as possible:
- **Critical Issues**: Within 1-2 weeks of resolution
- **High Severity**: Within 2-4 weeks of resolution
- **Medium Severity**: Within 4-8 weeks of resolution
- **Info**: Within 6-12 weeks of resolution

*Note: Payment times may vary based on team availability and complexity*



## Reporting Questions

### How do I submit a report?
**It's super simple!**

1. **Go to**: [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)
2. **Click**: "New Issue"
3. **Choose**: "Bug Report" template
4. **Fill in**: What you found, where it is, how to reproduce it
5. **Submit**: That's it!

**No complex forms, no email templates, no PGP keys - just a simple GitHub issue!**

### What should I include in my report?
- Clear description of the vulnerability
- Where it's located (which part of the system)
- How to reproduce the issue
- Any evidence (screenshots, code, videos)
- Your contact information for rewards

### How long does it take to get a response?
We aim to respond to all reports as quickly as possible:
- **Critical Issues**: Within 1-3 days
- **High Severity**: Within 3-7 days
- **Medium Severity**: Within 1-2 weeks
- **Info**: Within 1-2 weeks

*Note: Response times may vary based on team availability*

## Security Questions

### Is my testing legal?
Yes, as long as you follow our program rules and scope. We provide safe harbor for authorized testing within our defined scope.

### What if I find a critical vulnerability?
1. **Don't exploit it further** beyond proof of concept
2. **Report it immediately** via GitHub issue
3. **Don't publicly disclose** until we coordinate
4. **Follow our responsible disclosure timeline**

### Can I collaborate with other researchers?
Yes! Multiple researchers can work together. Just make sure to:
- List all contributors in the report
- Agree on reward distribution beforehand
- Document individual contributions clearly

## Technical Questions

### How do I set up a testing environment?
Follow our [Testing Guide](TESTING_GUIDE.md) which includes:
- Environment setup instructions
- Required tools and dependencies
- Testing methodology
- Common vulnerability examples

### What tools should I use?
We recommend:
- **Smart Contracts**: Slither, Mythril, Echidna
- **Web Apps**: OWASP ZAP, Burp Suite
- **APIs**: Postman, custom scripts
- **Infrastructure**: Cloud security tools

### Can I get help with testing?
Yes! Join our telegram channel for:
- Technical support
- Tool recommendations
- Collaboration opportunities
- Mentorship from experienced researchers

## Recognition Questions

### Will I be publicly acknowledged?
Yes! We publicly acknowledge researchers in security advisories. You can choose to remain anonymous if preferred.

### Are there special rewards?
Yes! We offer bonus considerations for:
- **Excellent documentation**: May increase reward tier
- **Working proof of concept**: May increase reward tier
- **Novel attack vectors**: May increase reward tier
- **First report**: May receive additional recognition

### Can I win monthly/annual awards?
Yes! We have recognition programs:
- **Monthly**: Researcher of the Month, Best Report, Most Innovative
- **Annual**: Researcher of the Year, Lifetime Achievement, Innovation Award

## Program Questions

### How often is the program updated?
We review and update the program based on:
- Researcher feedback
- Security landscape changes
- Program effectiveness metrics
- Scope expansion needs

*Next review: October 2025*

### Can I appeal a decision?
Yes! You can appeal within 30 days if you believe:
- Severity was misclassified
- Technical assessment was incorrect
- Scope determination was wrong
- Report quality wasn't properly recognized

### How transparent is the program?
We publish:
- Program statistics when available
- Vulnerability type distribution
- Resolution times
- Total rewards distributed
- Researcher satisfaction scores

## Support Questions

### How can I get help?
- **GitHub Issues**: [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)
- **Telegram**: [Dex223 Security Channel](https://t.me/Dex223_defi)
- **Discord**: [Dex223 Community](https://discord.gg/t5bdeGC5Jk)
- **GitHub**: [EthereumCommonwealth](https://github.com/EthereumCommonwealth)

### Is there a community?
Yes! We have an active security community:
- **Telegram channel** with active members
- **Discord server** with active discussions
- **Community discussions** for Q&A
- **Code review sessions** for learning

### Can I suggest improvements?
Absolutely! We welcome feedback on:
- Program rules and scope
- Reward structure
- Documentation and guides
- Community features
- Tool recommendations

## Emergency Questions

### What if I find a critical vulnerability being exploited?
1. **Open a GitHub issue immediately** with "CRITICAL" in the title
2. **Don't publicly disclose** the vulnerability
3. **Provide minimal details** needed for immediate response
4. **Follow our coordinated disclosure process**

### What if my report is urgent?
For urgent issues:
- Open a GitHub issue with "URGENT" in the title
- Post in Telegram channel (for critical issues only)
- We'll respond as quickly as possible

### What if I accidentally cause damage?
1. **Stop testing immediately**
2. **Contact us right away**
3. **Document what happened**
4. **Cooperate with our investigation**
5. **We'll work with you** to understand and prevent future issues

---

**Still have questions?** Open a [GitHub issue](https://github.com/rroland10/dex223-bug-bounty/issues) or join our Telegram/Discord community!

*Last Updated: July 2025* 