# Purpose

Ensure risk from software vulnerabilities remains within ORGANIZATION_NAME’s appetite and tolerance, or that the RISK_ACCEPTANCE_AUTHORITY affirmatively approves the acceptance or transfer of such excess risk.

# Scope
This policy applies to all organization-controlled code.

# Risk Mitigation or Avoidance
- The risk appetite of ORGANIZATION_NAME is RISK_APPETITE CURRENCY_UNITS per year.
- The risk tolerance of ORGANIZATION_NAME is RISK_TOLERANCE CURRENCY_UNITS.
- The RISK_ACCEPTANCE_AUTHORITY shall:

| Action | Timeline | Trigger|
|---|---|---|
|Identify, in writing via the ASSET_REGISTRY_LOCATION, a mutually exclusive and completely exhaustive list of assets under the control of the RISK_ACCEPTANCE_AUTHORITY.|15 calendar days|Enactment of policy, assumption of role, or creation of new asset|
|Identify, in writing via the ASSET_REGISTRY_LOCATION, the CURRENCY_UNIT asset value for every asset identified in the above step.|15 calendar days|Completion of above step|
|Ensure triage of all potential security vulnerabilities. Triage is complete when the RISK_ACCEPTANCE_AUTHORITY has ensured the written recording in VULNERABILITY_REGISTRY_LOCATION of assessments regarding:<br>- the probability of exploitation;<br> the asset or assets that would be impacted in the case of such exploitation;<br> - the exposure factor of each asset, separated by data attribute; and<br> - the annualized loss expectancy resulting from a given vulnerability.|72 hours|Detection of potential vulnerability|
|Ensure the probability of exploitation of every identified vulnerability is reviewed and documented in VULNERABILITY_REGISTRY_LOCATION.|7 calendar days|Completion of above step|
|Ensure the mitigation or avoidance of risk stemming from vulnerabilities, and document such actions in VULNERABILITY_REGISTRY_LOCATION.|As needed to avoid exceeding risk tolerance.|Determination that current risk exceeds risk appetite.|
|Ensure the preservation of all written entries in ASSET_REGISTRY_LOCATION and VULNERABILITY_REGISTRY_LOCATION.|7 calendar years|Entry of information|

- The PRIMARY_RISK_ADVISOR shall:

|Action|Timeline|Trigger|
|---|---|---|
|Designate appropriate methods for determining this probability of exploitation, which can include the use of commercial or open source automated tools. Document this in the EXPLOITABILITY_DETERMINATION_REGISTRY|7 calendar days|Enactment of policy, assumption of role, or identification of new method|

# Risk Acceptance or Transfer
- The RISK_ACCEPTANCE_AUTHORITY shall:

| Action | Timeline | Trigger |
|---|---|---|
|State in writing via VULNERABILITY_REGISTRY_LOCATION:<br>A plan, including timeline, for return to risk appetite; or<br>intention to accept or transfer the risk from vulnerabilities if, in the written opinion of the RISK_ACCEPTANCE_AUTHORITY, doing so is in the best interests of ORGANIZATION_NAME. In the latter case, such a statement shall include:<br>- Vulnerabilities for which risk is to be accepted or transferred;<br>- If risk is transferred, how it is being done (contractually, through insurance, etc.);<br>- Planned communication external to ORGANIZATION_NAME, if any;<br>- Justification for acceptance or transfer; and<br>- Plan, including timeline, for return to risk appetite, if applicable.|80% of risk tolerance expended or 72 hours, whichever is less|70% or more of risk tolerance expended|
|Approve deferral of applying controls to vulnerabilities in writing via VULNERABILITY_REGISTRY_LOCATION.|100% of risk tolerance expended or 72 hours after receipt of opinion from PRIMARY_RISK_ADVISOR, whichever is less|Receipt of opinion from PRIMARY_RISK_ADVISOR|
|When requesting an indefinite risk acceptance, conduct all above steps again, indefinitely or until risk in excess of appetite is mitigated or avoided.|180 calendar days after above step|174 calendar days after above step|	

- The PRIMARY_RISK_ADVISOR shall:

|Action|Timeline|Trigger|
|---|---|---|
|State, in writing via VULNERABILITY_REGISTRY_LOCATION, an opinion as to:<br> - The potential impact of exceeding the risk appetite in cybersecurity, regulatory, and reputational terms; and<br> - The feasibility of the RISK_ACCEPTANCE_AUTHORITY’s plan to return to ORGANIZATION_NAME’s risk appetite.|75% of risk tolerance expended or 72 hours, whichever is less|Receipt of statement from RISK_ACCEPTANCE_AUTHORITY|

# Compliance
- Non-compliance with this policy may result in disciplinary action, up to and including termination.
- The RISK_ACCEPTANCE_AUTHORITY shall:

|Action|Timeline|Trigger|
|---|---|---|
|Ensure the completion and documentation of a root cause analysis (RCA) in ROOT_CAUSE_ANALYSIS_REGISTRY_LOCATION.|7 calendar days|Identification of instance of non-compliance|
|Notify the POLICY_APPROVER in writing of each such case of noncompliance, as well as the results of the RCA.|3 calendar days|Completion of RCA.|
|Ensure every member of ORGANIZATION_NAME is retrained on this policy.|14 calendar days|Identification of 2 instances of non-compliance within 6 calendar month period|

# Definitions

* Data attributes: the confidentiality, integrity, and availability of information.

* Organization-controlled code: Computer language of any type which a properly authenticated and authorized member (employee or contractor) of the organization can wholly move into and out of operation without further coordination with anyone external to the organization.
   * This would include a company-built application, including any third-party libraries included therein, running on top of a Platform-as-a-Service offering.
   * This would exclude a Software-as-a-Service product, as company personnel cannot wholly move it into and out of operation themselves.

* Financial loss: the cost of something occurring to an organization. This does not merely include direct losses due to forgone revenue, but also reputational damage, unplanned employee attrition, regulatory action, and litigation, among other consequences.

* Vulnerability: any aspect of code that would allow a malicious actor to impact the attributes of data handled by it in a way that would cause financial loss to the organization.

* Probability of exploitation: in the opinion of a person or output of a tool designated by PRIMARY_RISK_ADVISOR, the likelihood that a malicious actor will exploit a given vulnerability in the next 365.24 days, recorded as a number between 0 and 1.0.

* Asset value: the financial loss over a 365.24 day period that would be suffered by the company after a completely successful malicious attack against a given asset. Each asset value shall include separate values for each data attribute.

* Exposure factor: The degree to which successful malicious exploitation of a given vulnerability will cause a loss to a given asset, recorded as a number between 0 and 1.0 for each data attribute.

* Annualized Loss Expectancy: A given vulnerability’s probability of exploitation multiplied by its exposure factor for each data attribute multiplied by potentially impacted asset values, for each data attribute.
