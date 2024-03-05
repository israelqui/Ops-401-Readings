# Reading 42
# Pass the Hash with Mimikatz
## Why is this topic important?

Mimikatz is a critical topic in cybersecurity as it represents a potent tool used by attackers to steal credentials, escalate privileges, and move laterally within compromised networks. Exploiting vulnerabilities in Windows authentication mechanisms, Mimikatz underscores the importance of addressing these security gaps and implementing robust defense strategies. Understanding Mimikatz enables defenders to develop effective mitigation techniques, such as implementing security controls like Credential Guard, monitoring for suspicious activity, and educating users about phishing tactics. Given its widespread use by threat actors, familiarity with Mimikatz is essential for cybersecurity professionals to detect, respond to, and mitigate credential theft attacks effectively.

## 

1. Name the six credential-gathering techniques which Mimikatz is able to perform and explain how two of them work.

    1. Pass-the-Hash (PtH): This technique involves stealing the NTLM password hashes stored in memory, often from LSASS (Local Security Authority Subsystem Service) process, and then using these hashes to authenticate as the user without needing to know their plaintext password. Once an attacker obtains these hashes, they can perform lateral movement within a network, accessing resources as if they were the compromised user.

    2. Pass-the-Ticket (PtT): In this technique, Mimikatz extracts Kerberos tickets from memory, which are used in Windows authentication for accessing network resources. Attackers can reuse these tickets to gain unauthorized access to network services without needing to know the user's password. By stealing and replaying these tickets, attackers can impersonate legitimate users and move laterally across the network.

    3. Over-Pass-the-Hash: This technique allows an attacker to overwrite a user's current NTLM hash with another hash, effectively changing the password for that user without knowing the original password.

    4. Pass-the-Certificate: This involves extracting X.509 certificates stored in memory, which can be used for authentication purposes. Attackers can reuse these certificates to impersonate legitimate users and gain access to network resources.

    5. Pass-the-Key: This technique involves stealing cached Kerberos keys from memory, which are used for authenticating to Kerberos-enabled services. Attackers can use these stolen keys to authenticate as legitimate users and access network resources.

    6. Pass-the-Cache: Mimikatz can also extract cached credentials from memory, including plaintext passwords, which are stored by various Windows authentication protocols. These credentials can then be reused to authenticate as the compromised user.

        Pass-the-Hash (PtH) and Pass-the-Ticket (PtT) are two of the most commonly used techniques by attackers.

        1. In Pass-the-Hash (PtH), once an attacker gains administrative privileges on a system, they can use tools like Mimikatz to extract the NTLM password hashes from the memory of the LSASS process. These hashes can then be used to authenticate to other systems on the network without needing the actual plaintext passwords. This works because Windows systems use NTLM hashes for authentication, and if an attacker has the hash, they can pass it along as if it were the actual password.

        2. In Pass-the-Ticket (PtT), Mimikatz extracts Kerberos tickets from memory, which are used for authentication in a Windows domain environment. Kerberos tickets contain encrypted authentication data that can be used to access various network resources without needing to provide a username and password. Mimikatz allows attackers to steal these tickets from memory and then reuse them to authenticate to other systems within the network, effectively impersonating legitimate users.


2. What are four ways we can defend against Mimikatz attacks. Explain how two of the mitigations can stop Mimikatz.

    1. Implement Credential Guard: Credential Guard is a Windows 10 security feature that helps protect credentials by utilizing virtualization-based security to isolate and secure the LSASS process in a secure enclave. This prevents Mimikatz from directly accessing and extracting sensitive credential information from memory, making it significantly more difficult for attackers to perform credential theft attacks.

    2. Enable Windows Defender Credential Guard: Similar to Credential Guard, Windows Defender Credential Guard (WD Credential Guard) also utilizes virtualization-based security to protect sensitive credential information from unauthorized access. It helps prevent Mimikatz and other similar tools from extracting plaintext credentials or hashes from memory by securely storing them in a virtualized environment that is isolated from the rest of the operating system.

    3. Implement Least Privilege Access: Restricting users' permissions to only what is necessary for their roles and responsibilities can help limit the potential impact of Mimikatz attacks. By reducing the number of accounts with administrative privileges and implementing the principle of least privilege, organizations can minimize the attack surface and make it more difficult for attackers to gain elevated privileges and access sensitive systems or data.

    4. Monitor for Anomalous Activity: Implementing robust monitoring and detection mechanisms can help identify and respond to Mimikatz attacks in real-time. This includes monitoring for suspicious or unusual behavior such as unauthorized access attempts, abnormal authentication patterns, and attempts to access sensitive systems or resources. By continuously monitoring for signs of compromise, organizations can detect and mitigate Mimikatz attacks before they result in data breaches or other security incidents.

        Two of these mitigations, Credential Guard and Windows Defender Credential Guard, effectively prevent Mimikatz attacks by utilizing virtualization-based security to protect sensitive credential information from unauthorized access:

        1. Credential Guard: By isolating and securing the LSASS process in a secure enclave using virtualization-based security, Credential Guard prevents Mimikatz from directly accessing and extracting sensitive credential information from memory. Even if an attacker gains access to the system, they won't be able to retrieve plaintext passwords or hashes, significantly mitigating the risk of credential theft.

        2. Windows Defender Credential Guard: Similar to Credential Guard, Windows Defender Credential Guard enhances the security of credential information by securely storing it in a virtualized environment that is isolated from the rest of the operating system. This prevents Mimikatz and other credential theft tools from accessing sensitive credential information, making it much more difficult for attackers to perform credential theft attacks.

## Analogy

Mimikatz can be likened to a master key that unlocks multiple doors within a building. Just as a master key grants access to various rooms, Mimikatz enables attackers to unlock sensitive information stored in different systems within a network by exploiting vulnerabilities in authentication mechanisms. Like a skilled intruder, Mimikatz bypasses traditional security measures, gaining entry and navigating freely across the network, posing a significant threat to the integrity and confidentiality of organizational data.

## Things i want to know more about:
- Technical aspects of how Mimikatz works. This could involve studying its source code, understanding its various commands and options, and exploring its capabilities in detail.
- Attack scenarios where Mimikatz can be used, such as Pass-the-Hash, Pass-the-Ticket, Over-Pass-the-Hash, and others
- Real-world incidents and case studies where Mimikatz was used in cyber attacks.
## Sources:
- https://www.varonis.com/blog/what-is-mimikatz/
- https://chat.openai.com/
