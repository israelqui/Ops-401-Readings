# Reading 16
# Cloud Identity and Access Management (IAM) with AWS
## Why is this topic important

Understanding and learning from the Capital One data breach is crucial for several reasons. Firstly, it serves as a real-world case study that highlights the potential vulnerabilities in cloud security, specifically within AWS environments. By dissecting the incident, individuals and organizations can gain insights into common attack vectors, such as server-side request forgery (SSRF), and the importance of robust access controls. Learning from this breach helps strengthen cybersecurity practices, emphasizing the need for vigilance in configuring and monitoring cloud infrastructure. Moreover, insights from such incidents contribute to the ongoing evolution of best practices, enabling the broader community to better safeguard sensitive data and mitigate the impact of potential future breaches.

1. What were the three commands used for the attack?

    1. Command to fetch data:
    The attacker used an SSRF vulnerability to issue a command instructing the server to fetch sensitive data from Capital One's storage.

    2. Command to exfiltrate data:
    After successfully fetching the desired data, the attacker issued a command to exfiltrate or export the stolen information.

    3. Command to persist data:
    The attacker may have used another command to ensure that the stolen data was persistently stored or accessible for future unauthorized access.

2. What misconfiguration of AWS components allowed the attacker to access sensitive data?

    1. Server-Side Request Forgery (SSRF): The attacker exploited a vulnerability that allowed them to send requests from the web server to the metadata service of the underlying AWS instance. This metadata service is intended to provide information about the instance, such as its configuration and associated IAM (Identity and Access Management) roles.

    2. Access to IAM Roles: The SSRF vulnerability allowed the attacker to gain access to the AWS IAM role associated with the compromised instance. The IAM role had overly permissive permissions, allowing it to access sensitive information stored in AWS S3 buckets.

    3. Data Retrieval: Using the compromised IAM role, the attacker issued commands to the AWS metadata service to retrieve sensitive data stored in Capital One's S3 buckets. This data included personal information of Capital One customers.



3. What are two of the AWS Governance practices that could have prevented such attack?

    - Principle of Least Privilege (PoLP):
    Enforce the principle of least privilege for AWS IAM roles and permissions. In the Capital One case, the attacker gained unauthorized access to sensitive data through a misconfigured IAM role with overly permissive permissions. By strictly adhering to the principle of least privilege, organizations can ensure that each IAM entity (user, group, or role) has the minimum level of permissions necessary to perform its intended tasks. Regularly review and audit IAM policies to eliminate unnecessary privileges, reducing the attack surface and the potential impact of security incidents.

    - AWS Security Best Practices and Well-Architected Framework:
    Follow AWS security best practices and leverage the AWS Well-Architected Framework. AWS provides comprehensive documentation and guidance on best practices for securing cloud environments. The Well-Architected Framework covers key pillars, including Security, and offers guidelines for designing, deploying, and maintaining secure and efficient workloads on AWS. By conducting regular reviews using the Well-Architected Framework, organizations can identify and address security vulnerabilities, misconfigurations, and other potential risks in their AWS environments. This proactive approach helps organizations maintain a strong security posture and reduces the likelihood of successful attacks.

## Analogy

Imagine a library where patrons use a computerized system to request books, and a mischievous individual exploits a flaw in the system to make unauthorized book requests, akin to a Server-Side Request Forgery (SSRF) attack. This reflects the vulnerability of allowing unintended actions through a system's weaknesses. A well-architected system, similar to a secure library setup, would enforce controlled access and implement security measures. It ensures that requests are processed through authorized channels and undergoes regular audits to identify and address potential vulnerabilities. This analogy highlights the importance of a robust architecture, following best practices, and conducting regular reviews to prevent unauthorized access and protect against potential data breaches in systems like those hosted on AWS.

## Things i want to learn more about?
Understand how the legal system responded to the incident, including charges filed against the perpetrator and any settlements or fines imposed on Capital One.

## Source:
- https://www.zscaler.com/resources/white-papers/capital-one-data-breach.pdf
- https://chat.openai.com/
