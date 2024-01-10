# Reading 3
# Cyber Risk Analysis

## Why is this topic important

Cyber risk analysis is crucial because it provides a structured approach to identifying, assessing, and mitigating potential threats and vulnerabilities in digital systems. It helps organizations understand their exposure to cyber threats, quantify the potential impact of these risks, and prioritize resources effectively. By conducting cyber risk analysis, businesses can proactively anticipate and prepare for potential cyberattacks, minimizing the likelihood of breaches, financial losses, reputational damage, and operational disruptions. It enables informed decision-making, allowing organizations to allocate resources efficiently towards robust security measures that align with their risk tolerance and business objectives.

1. Consider a bank ATM that allows users to access bank account balances. What measures can the ATM incorporate to cover the principles of the CIA triad?


An ATM can ensure the principles of the CIA triad by employing encryption for secure data transmission (Confidentiality), implementing data validation and transaction verification measures (Integrity), and maintaining redundant systems, regular upkeep, and physical security protocols (Availability). By encrypting communication, ensuring data integrity, and maintaining system availability through backups and maintenance, the ATM can safeguard sensitive information, prevent unauthorized access or alterations, and ensure uninterrupted service for users, covering the core principles of information security.

2. Name three best practices that support the CIA triad.

1. Confidentiality: Prevent unauthorized disclosure
Confidentiality of information refers to protecting the information from disclosure to unauthorized parties.


Key areas for maintaining confidentiality:


Social engineering: Training and awareness, defining separation of duties at the tactical level, enforcing policies and conducting vulnerability assessments
Media reuse: Proper sanitization strategies
Eavesdropping: Use of encryption and keeping sensitive information off the network with adequate access controls

2. Integrity: Detect modification of information

The integrity of information denotes protecting sensitive information from being modified by unauthorized parties.


Key areas for maintaining confidentiality:


- Implement encryption using integrity-based algorithms
- Prevent intentional or malicious modification (message digest, MAC, digital signatures)

3. Availability: Provide timely and reliable access to resources

Availability of information signifies ensuring that all the required or intended parties are able to access the information when needed.


Key areas for maintaining availability:


- Prevent single point of failure
- Comprehensive fault tolerance (data, hard drives, servers, network links, etc.)

3. What are the three stages of the risk management lifecycle? What is each stage’s main goal or objective?

1. Risk assessment

Looks at risks corresponding to identified parameters for a specific period and must be reevaluated periodically. Managing risks is an ongoing process. The following steps are officially part of a risk assessment as per NIST 800-30:

- System characterization
- Threat identification
- Vulnerability identification
- Control analysis
- Likelihood determination
- Impact analysis
- Risk determination
- Control recommendation
- Results documentation

2. Risk analysis

Risk can be analyzed through a qualitative and quantitative lens.


Qualitative analysis is subjective in nature and uses words like “high,” “medium,” “low” to describe the likelihood and severity of the impact of a threat exposing a vulnerability.


Quantitative analysis is objective and numbers-driven. It requires more experience than qualitative analysis and involves calculations to determine a dollar value associated with each risk element. Business decisions are fundamentally driven by this type of analysis. It is essential in order to conduct a cost/benefit analysis


Key pointers to be remembered for risk analysis include:

- AV: Asset value
- EF: Exposure factor
- ARO: Annual rate of occurrence
- Single loss expectancy = AV * EF
- Annual loss expectancy = SLE * ARO
- Risk value = probability * impact (Probability is how likely it is for the threat to materialize and impact the extent of the damage)

3. Mitigating risk

There are three acceptable responses to risk mitigation:

- Reduce
- Transfer
- Accept

Organizations need to continue to monitor for risks. How an organization decides to mitigate business risks becomes the basis for security governance and policy.

## Analogy

Cyber risk analysis is like checking your home's security before leaving for a trip. Just as you'd inspect doors, windows, and alarms to prevent burglaries, cyber risk analysis examines digital "doors" (like networks and systems) for potential weaknesses. It's akin to ensuring your locks are strong, windows are secure, and alarms are functional—identifying and addressing vulnerabilities before leaving. This proactive approach reduces the chance of a break-in while you're away, much like how cyber risk analysis reduces the likelihood of digital breaches in your absence, safeguarding your digital assets.

## Things I want to lean more about
- Understand various cyber threats and vulnerabilities in digital systems.
- Keeping up with with evolving threats.

## Sources:
- https://resources.infosecinstitute.com/certification/security-risk-management/
- https://chat.openai.com/

## Other links:
- https://www.cybersecurityeducation.org/careers/security-auditor/
- https://www.youtube.com/watch?v=1PVC-fwnxp4&ab_channel=UniversityofDayton
