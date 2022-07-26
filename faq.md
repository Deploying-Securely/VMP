# Frequently asked questions (FAQ)

**Question**: How do I determine my organization’s risk appetite and risk tolerance?

**Answer**: This will depend entirely on your line of business and the competitive, regulatory, and cybersecurity risks you face. Read this [article](https://haydock.substack.com/p/managing-your-risk-surface) on the topic as well as this [post](https://www.fairinstitute.org/blog/cyber-risk-management-establishing-a-blueprint-with-fair) from the FAIR Institute for more details on how to determine this.


**Question**: Should I use my organization’s total cyber risk appetite and risk tolerance?
**Answer**: No. You should only include your risk tolerance from software vulnerabilities (as defined in the policy). Risk from other things like insider threat, etc. should be counted separately.

**Question**: How do I determine the value of an asset?
**Answer**: Determining an asset’s value requires deep knowledge of your specific business, and depends on factors such as revenue that would be forgone, cost of replacing the asset, and less tangible factors such as reputation and goodwill. The Deploying Securely blog, FAIR Institute and RiskLens provide some guides on how to proceed.

**Question**: How do I determine the exposure factor for a given vulnerability?
**Answer**: Since the exposure factor represents the degree to which the attributes of data (confidentiality, integrity, availability) will be impacted as the result of a malicious attack, the exposure factor will vary greatly depending on the situation. For confidentiality, the exposure factor is generally 1.0, as one data is exposed or stolen, there is no way to “undo” the problem, and regulators generally take this view when assessing fines. If, however, it is possible to prevent half of the data from being stolen due to some compensating control (e.g. encryption), then the exposure factor could be 0.5. For integrity, if the data is permanently corrupted (e.g. following a successful ransomware attack), the exposure factor will likely be 1.0 as well. If, however, it is possible to repair the data for 5% of the total asset value, then the exposure factor would be 0.05. For availability, if a successful denial of service attack could completely shut down access to an eCommerce portal for 10 days (assuming no other action by the organization) out of the year, the exposure factor would be 0.027 (10 days divided by 365.24 days in a year).

**Question**: Why doesn’t the policy say anything about vulnerability scanning?
**Answer**: Vulnerability scanning and vulnerability management are two logically separate concepts. The first is a method of risk assessment while the second is a method of risk management. The frequency of vulnerability identification will generally increase when an organization scans for vulnerabilities more often or does so using more tools. Including requirements for such parameters in a vulnerability management policy, however, frequently causes organizations to conflate the concepts of risk assessment and management. In some cases, this has even led to engineering organizations advocating for (and security teams agreeing to) limiting scanning of certain code bases to reduce the frequency of vulnerability reports. Such actions are logically backward, and separating vulnerability scanning policies from vulnerability management ones helps to prevent such pressures.

**Question**: How do I determine the likelihood of exploitability?
**Answer**: This is a tricky question and there is no right answer. The Exploit Prediction Scoring System (EPSS) provides a good way to do this for published common vulnerabilities and exposures (CVE), but its output is only for the next 30 days, rather than 365.24 (one year). The Deploy Securely Risk Assessment Model (DSRAM) can annualize these figures, as well as provide estimates for non-CVE exploitability. Ultimately this will be a judgment call for your organization, but the aforementioned tools provide automated tools for estimating it.

**Question**: Why doesn’t the policy say anything about false positives?
**Answer**: This policy is meant to serve as a method for managing risk in probabilistic terms. It is difficult to ever confidently claim that there is “zero risk” from any given situation. With that said, there are situations where a scanning tool will report a vulnerability that, upon further analysis, has practically no chance of exploitation. In such a situation, those triaging it should assign a very low (or zero) percentage chance of exploitation to this issue to reflect the reality of its low risk.

**Question**: Why doesn’t the PRIMARY_RISK_ADVISOR need to approve a risk acceptance or transfer?
Answer: Business leaders should make risk decisions and be ultimately accountable for them. Information security personnel - up to and including the Chief Information Security Officer of the organization - are, in the end, advisors and implementers. Thus, the role of the PRIMARY_RISK_ADVISOR in this policy template is to provide an opinion on the likely outcome of a given risk decision, but does not assume accountability for it, outside of the effectiveness of its implementation.

**Question**: What does it mean when risk tolerance is “expended”?
**Answer**: As an organization exceeds its risk appetite, its risk tolerance explains how quickly it must return to the pre-existing baseline. This speed will vary with how far in excess of the risk appetite the organization has veered. Using a dollar value for risk tolerance signifies that the organization is only allowed to “expend” or “incur” a certain amount of accrued risk before it must return to said baseline. Please review this article for a detailed description of this parameter.