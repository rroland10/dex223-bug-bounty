# Dex223 Bug Bounty Program Rules

## Program Overview

The Dex223 Bug Bounty Program is designed to identify and fix security vulnerabilities in our decentralized exchange platform. These guidelines ensure fair, ethical, and effective security research while maintaining professional conduct and responsible disclosure practices. As a decentralized team, we value flexibility and community-driven approaches.

## Eligibility

### Who Can Participate
- Security researchers, ethical hackers, and cybersecurity professionals
- Individuals aged 18 or older
- Residents of countries not subject to US sanctions
- Participants must comply with all applicable laws and regulations

### Who Cannot Participate
- Dex223 employees, contractors, and their immediate family members
- Individuals involved in the development of the reported vulnerability
- Participants from sanctioned countries
- Minors under 18 years of age

## Testing Guidelines

### Allowed Activities
- **Smart Contract Testing**: Static analysis, fuzzing, formal verification
- **Web Application Testing**: OWASP Top 10 vulnerabilities, API testing
- **API Endpoint Testing**: All public and authenticated APIs including Fiat on/off-ramp integration
- **Infrastructure Testing**: Cloud misconfigurations, deployment pipeline analysis
- **Social Engineering**: Phishing simulations (with prior approval)

### Prohibited Activities
- **Denial of Service**: DoS/DDoS attacks against production systems
- **Data Exfiltration**: Unauthorized access to user data beyond proof of concept
- **Destructive Testing**: Actions that could damage systems or data
- **Physical Security**: Attempts to gain physical access to facilities
- **Social Engineering**: Without explicit written permission
- **Third-Party Services**: Testing services not owned by Dex223

### Testing Environment
- **Production Systems**: Limited testing allowed with proper safeguards
- **Testnets**: Full testing encouraged for smart contracts
- **Staging Environment**: Available for comprehensive testing
- **Local Development**: Recommended for initial research
- **Test App**: https://test-app.dex223.io
- **Swap Interface**: https://test-app.dex223.io/en/swap

## Submission Requirements

### Report Format
All submissions should include:

1. **Clear Description**: What the vulnerability is
2. **Reproduction Steps**: How to reproduce the issue
3. **Impact**: What could happen if exploited
4. **Proof of Concept**: Evidence of the vulnerability (screenshots, code, etc.)
5. **Suggested Fix**: How you think it could be fixed

### Required Information
- **What you found**: Brief description of the vulnerability
- **Where it is**: Which part of the system is affected
- **How to test it**: Steps to reproduce the issue
- **Your contact info**: How we can reach you for rewards

### Submission Channels
- **Primary**: [GitHub Issues](https://github.com/rroland10/dex223-bug-bounty/issues)
- **Backup**: GitHub Security Advisories
- **Emergency**: Telegram security channel (for critical issues)

## Response Timeline

### Initial Response
We aim to respond to all reports as quickly as possible, typically:
- **Critical Issues**: Within 24-48 hours
- **High Severity**: Within 3-5 business days
- **Medium Severity**: Within 1-2 weeks
- **Info**: Within 1-2 weeks

### Resolution Timeline
Resolution times may vary based on complexity and team availability:
- **Critical Issues**: As soon as possible, typically 1-2 weeks
- **High Severity**: 2-4 weeks
- **Medium Severity**: 4-8 weeks
- **Info**: 6-12 weeks

### Communication
- Status updates via GitHub issue comments
- Public disclosure coordination
- Researcher acknowledgment in security advisories

## Reward Criteria

### Severity Assessment
Rewards are determined based on:
- **Impact**: Potential damage and affected users
- **Exploitability**: Difficulty of exploitation
- **Scope**: Number of affected systems
- **Novelty**: Uniqueness of the vulnerability

### Reward Tiers
Rewards are paid in D223 tokens:
- **Critical**: 30M D223 - A vulnerability that can completely break the contracts workflow
- **High**: 7M D223 - A bug report that indicates a high severity problem but can't impact the whole platform
- **Medium**: 3M D223 - A low-severity problem that can lead to a loss of funds but under specific conditions
- **Info**: 1M D223 - Anything else - best practices, documentation improvements, etc.

### Bonus Factors
- **First Report**: May receive additional recognition
- **Quality**: Comprehensive and well-documented reports may increase reward tier
- **Innovation**: Novel attack vectors or techniques may increase reward tier
- **Responsibility**: Following disclosure guidelines

### Disqualification
Reports may be disqualified for:
- Violation of testing guidelines
- Incomplete or inaccurate information
- Duplicate submissions
- Non-reproducible issues
- Out-of-scope vulnerabilities

## Duplicate Handling

### Duplicate Policy
- **First Valid Report**: Receives full reward
- **Subsequent Reports**: May receive partial credit if significant additional information
- **Collaborative Reports**: Rewards split among researchers
- **Timeline**: Reports within 24-48 hours of each other may be considered simultaneous

### Collaboration Guidelines
- Multiple researchers can work together
- All contributors should be listed in the report
- Reward distribution should be agreed upon beforehand
- Individual contributions should be clearly documented

## Program Metrics

### Transparency
- Program statistics when available
- Vulnerability type distribution
- Resolution times
- Total rewards distributed
- Researcher participation metrics

### Continuous Improvement
- Rule updates based on community feedback
- Program effectiveness evaluation
- Scope expansion based on needs
- Reward structure adjustments

## Legal Framework

### Responsible Disclosure
- Coordinated disclosure timeline for critical vulnerabilities
- Public acknowledgment of researchers
- No legal action for good-faith testing

### Legal Protection
- Safe harbor for authorized testing within defined scope
- Protection against legal retaliation for good-faith research
- Clear scope definition and testing boundaries
- Compliance with applicable laws and regulations
- Intellectual property protection for researchers

### Intellectual Property
- Researchers retain rights to their findings
- Dex223 may use findings for security improvements
- Public disclosure coordination
- Attribution in security advisories

## Support and Communication

### Contact Information
- **Security Team**: contact@dex223.io
- **Emergency**: Telegram security channel
- **Telegram**: [Dex223 Security Channel](https://t.me/Dex223_defi)
- **Discord**: [Dex223 Community](https://discord.gg/t5bdeGC5Jk)
- **GitHub Issues**: [https://github.com/rroland10/dex223-bug-bounty/issues](https://github.com/rroland10/dex223-bug-bounty/issues)

### Communication Channels
- **Primary**: GitHub Issues for all reports and questions
- **Updates**: GitHub Security Advisories
- **Community**: Telegram and Discord servers
- **Public**: Security blog and social media
- **Repository**: [EthereumCommonwealth](https://github.com/EthereumCommonwealth)

## Program Updates

### Version Control
- Rule changes tracked in version control
- Change notifications to registered researchers when possible
- Community input on significant changes
- Flexibility for ongoing investigations

### Feedback Process
- Researcher feedback collection
- Community-driven program reviews
- Community input solicitation
- Continuous improvement implementation

---

**Last Updated**: July 2025  
**Version**: 1.0  
**Next Review**: October 2025 