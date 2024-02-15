# Reading 29
# Modeling a Web Application
## Why is this topic important?

Integrating threat modeling is essential because it enables us to identify and mitigate security risks early, protecting our application, users, and reputation. By proactively addressing vulnerabilities, we uphold trust, comply with regulations, minimize costs, and foster a culture of security within our team, ensuring the delivery of a reliable, high-quality product.

##

1. Explain threat modeling using real-world non-technical examples.

    Threat modeling is a structured approach to identifying, evaluating, and prioritizing potential threats and vulnerabilities in a system or environment. While it's commonly associated with technical systems like software or networks, the principles of threat modeling can also be applied to non-technical, real-world scenarios. Here are some examples:

    1. Home Security:

        Scenario: You want to improve the security of your home.
        Threat Model: Identify potential threats such as burglary, fire, or natural disasters.
        Mitigation Strategies: Install deadbolts, security cameras, smoke detectors, and have an evacuation plan in case of emergencies.
    2. Personal Safety:

        Scenario: You're walking alone at night in an unfamiliar area.
        Threat Model: Potential threats include mugging, assault, or getting lost.
        Mitigation Strategies: Stay in well-lit areas, avoid distractions like headphones, share your location with a friend, and be aware of your surroundings.
    3. Financial Security:

        Scenario: You're managing your finances.
        Threat Model: Threats could include identity theft, fraud, or unexpected expenses.
        Mitigation Strategies: Use strong, unique passwords for online accounts, monitor bank statements regularly for suspicious activity, enable two-factor authentication where possible, and maintain an emergency fund.
    4. Travel Safety:

        Scenario: You're planning a trip to a foreign country.
        Threat Model: Consider threats such as theft, scams, health emergencies, or natural disasters.
        Mitigation Strategies: Research the destination for potential risks, purchase travel insurance, keep important documents secure, stay updated on local news and advisories, and have a communication plan in case of emergencies.
    5. Business Operations:

        Scenario: You're running a small business.
        Threat Model: Threats may include competition, supply chain disruptions, data breaches, or economic downturns.
        Mitigation Strategies: Diversify your supply chain, regularly backup critical data, implement cybersecurity measures, have a contingency plan for emergencies, and stay informed about industry trends.

2. What are the four questions that can help us organize threat modeling?


    - "STRIDE":

        - Spoofing:
            Can someone pretend to be something they're not? This involves unauthorized access by assuming the identity of another user, system, or entity.
        - Tampering:
            Can someone maliciously modify data or systems? This refers to unauthorized alterations to data, configurations, or code that can compromise the integrity of a system.
        - Repudiation:
            Can someone deny performing a specific action? This involves the inability to verify the actions or transactions of a user or entity, leading to disputes or denial of responsibility.
        - Information disclosure:
            Can someone access information they're not supposed to? This encompasses the unauthorized exposure or leakage of sensitive data, potentially leading to privacy breaches or loss of confidentiality.
        - Denial of Service (DoS):
            Can someone prevent legitimate users from accessing resources or services? This involves attacks aimed at disrupting or degrading the availability of a system or service, rendering it unusable for its intended users.
        - Elevation of Privilege:
            Can someone gain unauthorized access to elevated permissions or privileges? This involves exploiting vulnerabilities to gain higher levels of access or control than intended, potentially leading to unauthorized actions or compromises.


3. You are the project lead for a new application. How would you explain the benefits of Threat Modeling to the rest of the team?

    - Risk Reduction: By systematically identifying and analyzing potential threats, we can proactively implement countermeasures to mitigate risks before they manifest into security incidents. This helps us reduce the likelihood and impact of security breaches, protecting our application and its users.

    - Cost Savings: Addressing security vulnerabilities early in the development process is much more cost-effective than addressing them after the application has been deployed. By investing in threat modeling upfront, we can avoid costly security fixes and potential damages resulting from security breaches down the line.

    - Enhanced Security Awareness: Engaging in threat modeling encourages the team to think critically about security throughout the development process. It raises awareness about common security threats and vulnerabilities, empowering team members to make informed decisions and write more secure code.

    - Compliance and Assurance: Many regulatory standards and industry best practices require organizations to demonstrate that they have considered security risks in their applications. Incorporating threat modeling helps us meet these compliance requirements and provides assurance to stakeholders, including customers and regulatory bodies, that we take security seriously.

    - Improved Collaboration: Threat modeling is a collaborative exercise that involves input from various stakeholders, including developers, architects, and security experts. By engaging in threat modeling workshops or discussions, we foster collaboration across different teams and disciplines, leading to a more holistic understanding of security risks and better-informed security decisions.

    - Quality Assurance: Addressing security concerns early in the development process can also improve the overall quality of our application. By identifying potential vulnerabilities and weaknesses, we can implement more robust and resilient designs, leading to a more reliable and trustworthy product.

## Things i want to know more about:
- Continuous Integration/Continuous Deployment (CI/CD)
## Sources:
- https://owasp.org/www-community/Application_Threat_Modeling
- https://www.ockam.io/learn/blog/introduction_to_STRIDE_security_model
- https://docs.microsoft.com/en-us/learn/paths/tm-threat-modeling-fundamentals/ 
- https://chat.openai.com/
