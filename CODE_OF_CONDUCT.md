# Dex223 Bug Bounty Code of Conduct

## Our Commitment

Dex223 is committed to fostering an inclusive, respectful, and collaborative environment for all participants in our bug bounty program. This code of conduct outlines our expectations for behavior and the consequences for unacceptable conduct. As a decentralized team, we value community-driven approaches and flexibility.

## Expected Behavior

### Professional Conduct
- **Respect**: Treat all participants with respect and dignity
- **Collaboration**: Work constructively with other researchers and our team
- **Honesty**: Provide accurate and truthful information in reports
- **Responsibility**: Follow responsible disclosure practices
- **Learning**: Share knowledge and help others improve

### Communication Standards
- **Clear**: Use clear, professional language in all communications
- **Constructive**: Provide helpful feedback and suggestions
- **Timely**: Respond to requests and updates when possible
- **Appropriate**: Keep discussions focused on security research
- **Respectful**: Avoid personal attacks or inflammatory language

### Research Ethics
- **Scope Compliance**: Only test systems within the defined scope
- **Minimal Impact**: Minimize any potential damage during testing
- **Documentation**: Thoroughly document findings and methodologies
- **Coordination**: Coordinate disclosure with our security team
- **Improvement**: Focus on helping improve security, not just finding bugs

## Unacceptable Behavior

### Prohibited Actions
- **Harassment**: Any form of harassment, bullying, or intimidation
- **Discrimination**: Discrimination based on race, gender, age, religion, etc.
- **Threats**: Threats of violence or harm to individuals or systems
- **Malicious Testing**: Testing designed to cause damage or disruption
- **Unauthorized Access**: Accessing systems outside the defined scope

### Communication Violations
- **Inappropriate Language**: Offensive, vulgar, or discriminatory language
- **Spam**: Excessive or irrelevant messages
- **False Reports**: Submitting false or misleading vulnerability reports
- **Public Shaming**: Publicly shaming or attacking other researchers
- **Confidentiality Breaches**: Sharing confidential information without permission

### Research Violations
- **Scope Violations**: Testing systems not included in the program scope
- **Destructive Testing**: Actions that could damage systems or data
- **Unauthorized Disclosure**: Public disclosure before coordination
- **Exploitation**: Exploiting vulnerabilities beyond proof of concept
- **Social Engineering**: Social engineering attacks without permission

## Reporting Violations

### How to Report
If you experience or witness unacceptable behavior:

1. **Immediate**: Open a [GitHub issue](https://github.com/rroland10/dex223-bug-bounty/issues) with "CONDUCT VIOLATION" in the title
2. **Emergency**: Use our Telegram channel for urgent issues
3. **Anonymous**: Submit anonymous reports through our feedback form
4. **Escalation**: Contact community moderators if needed

### What to Include
- **Description**: Clear description of the incident
- **Evidence**: Screenshots, logs, or other supporting evidence
- **Witnesses**: Names of any witnesses (if comfortable sharing)
- **Timeline**: When the incident occurred
- **Impact**: How it affected you or others

### Investigation Process
1. **Acknowledgment**: We'll acknowledge receipt when possible
2. **Investigation**: Community-driven investigation of the reported incident
3. **Community Input**: Gathering input from community members
4. **Decision**: Making a fair and community-driven decision
5. **Action**: Taking appropriate corrective action
6. **Follow-up**: Ensuring the issue is resolved

## Consequences

### Warning System
- **First Violation**: Community discussion and education
- **Second Violation**: Temporary suspension from program
- **Third Violation**: Permanent removal from program
- **Severe Violation**: Immediate removal and community action if necessary

### Specific Consequences
- **Scope Violations**: Community review and potential suspension
- **Harassment**: Zero tolerance - immediate removal
- **Malicious Testing**: Permanent ban and community action
- **False Reports**: Warning and potential suspension
- **Confidentiality Breaches**: Immediate removal and community action

### Appeal Process
- **Right to Appeal**: All participants have the right to appeal decisions
- **Timeline**: Appeals should be submitted within 30 days
- **Review**: Community review and input
- **Final Decision**: Community-driven decision after appeal review

## Positive Recognition

### Good Conduct Rewards
- **Community Helper**: Recognition for helping other researchers
- **Mentorship**: Opportunities to mentor new participants
- **Leadership**: Invitations to community advisory roles
- **Recognition**: Public acknowledgment of positive contributions

### Examples of Positive Behavior
- **Helping Newcomers**: Assisting new researchers with setup and questions
- **Knowledge Sharing**: Sharing tools, techniques, and best practices
- **Constructive Feedback**: Providing helpful feedback on reports
- **Community Building**: Contributing to a positive community culture
- **Innovation**: Developing new tools or methodologies

## Continuous Improvement

### Feedback Collection
- **Community Feedback**: Regular community input on program culture
- **Suggestion Box**: Open channel for improvement suggestions
- **Community Discussions**: Regular discussions on program culture
- **Anonymous Feedback**: Anonymous channels for sensitive feedback

### Policy Updates
- **Community Review**: Community input on code of conduct updates
- **Community Input**: Incorporating community feedback
- **Best Practices**: Following community best practices
- **Transparency**: Clear communication about policy changes

## Support Resources

### Immediate Support
- **Security Team**: [GitHub Issues](https://github.com/rroland10/dex223-bug-bounty/issues)
- **Telegram Moderation**: Community moderators in Telegram
- **Discord Moderation**: Community moderators in Discord
- **GitHub**: [EthereumCommonwealth](https://github.com/EthereumCommonwealth)
- **Anonymous Reporting**: Community feedback channels

### External Resources
- **Mental Health**: Crisis hotlines and counseling services
- **Legal Support**: Information about legal rights and options
- **Community Support**: Peer support groups and networks
- **Professional Development**: Resources for career growth

## Our Values

### Core Principles
- **Security First**: Prioritizing the security of our platform and users
- **Community**: Building a supportive and collaborative community
- **Innovation**: Encouraging creative and innovative security research
- **Integrity**: Maintaining high ethical standards in all activities
- **Inclusion**: Welcoming participants from diverse backgrounds

### Commitment to Diversity
- **Equal Opportunity**: Equal access to program participation
- **Inclusive Environment**: Creating a welcoming environment for all
- **Community Representation**: Ensuring diverse community representation
- **Cultural Sensitivity**: Respecting different cultural backgrounds
- **Accessibility**: Making the program accessible to all participants

## Scope

### Smart Contract Source Codes
The bug bounty program covers the following smart contract source codes:
- **Repository**: [Dex223-contracts](https://github.com/EthereumCommonwealth/Dex223-contracts/tree/253367297d9093db21661b297cdbb104d8579e35)
- **Focus Areas**: All smart contracts within the defined scope, excluding specific modules listed below

## Out of Scope

### Excluded Modules
The following modules are explicitly out of scope for the bug bounty program:

- **MarginModule**: [Dex223MarginModule.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/253367297d9093db21661b297cdbb104d8579e35/contracts/dex-core/Dex223MarginModule.sol)
  - **Reason**: Work-in-progress module not ready for security testing
  
- **PriceOracle for MarginModule**: [Dex223Oracle.sol](https://github.com/EthereumCommonwealth/Dex223-contracts/blob/253367297d9093db21661b297cdbb104d8579e35/contracts/dex-core/Dex223Oracle.sol)
  - **Reason**: Oracle implementation specifically designed for the MarginModule

## Known Issues

The following issues are already known and should not be reported as new vulnerabilities:

1. **Pool Creation Error**: Error in pool creation for a token pair where one token is ERC-20 Original and the other is ERC-223 Original without an existing ERC-20 wrapper.

2. **Auto-conversion Issue**: Auto-conversion of ERC-20 wrapper-tokens to ERC-223 origin in a pair where one token is ERC-20 Origin and the other is ERC-223 Origin does not happen when there is only ERC-20-side liquidity in that pool.

---

**Together, we can create a safe, respectful, and productive environment for security research.**

*Last Updated: July 2025* 