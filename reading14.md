# Reading 14
# Intrusion Detention and Prevention Systems (IDS/IPS)
# Why is this topic important?

Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS) lies in their critical role in safeguarding digital environments from an ever-growing array of cyber threats. As technology advances, so do the techniques of malicious actors seeking to exploit vulnerabilities in networks and systems. IDS serves as a watchful guardian, detecting abnormal activities and potential security breaches early on. IPS takes this vigilance a step further by actively intervening to prevent identified threats from causing harm. In an era where cybersecurity is paramount, the deployment of effective IDS and IPS measures is essential for organizations to thwart cyber attacks, protect sensitive data, and maintain the integrity of their digital 

1. List 2 differences between firewalls and an IDS?


    1. Functionality:

    - Firewalls: Firewalls primarily focus on preventing unauthorized access to a network by monitoring and controlling incoming and outgoing network traffic. They act as a barrier between a trusted internal network and untrusted external networks, deciding whether to allow or block specific traffic based on predetermined security rules.

    - Intrusion Detection Systems (IDS): IDS, on the other hand, are designed to detect and respond to suspicious activities or potential security threats within a network. Instead of preventing access like firewalls, IDS monitor network or system activities in real-time, looking for patterns or behaviors that may indicate a security incident. IDS can be classified into two types: Network-based IDS (NIDS) and Host-based IDS (HIDS).

    2. Focus on Traffic:

    - Firewalls: Firewalls focus on controlling the flow of traffic based on pre-established rules. They make decisions about whether to allow or block traffic based on factors such as source and destination IP addresses, port numbers, and protocols. Firewalls are effective in preventing unauthorized access and protecting against certain types of cyber attacks.

    - Intrusion Detection Systems (IDS): IDS are more concerned with analyzing patterns and behaviors within the network traffic. They are less focused on making decisions about traffic flow and more on identifying potential security incidents. When an IDS detects suspicious activity, it generates alerts or takes other predefined actions to notify administrators or trigger automated responses.

2. Under what circumstances would you choose a network-based IDS over a host-based IDS?


Choosing between a network-based IDS (NIDS) and a host-based IDS (HIDS) depends on the specific security requirements and objectives of a system or network. A NIDS is typically preferred when the emphasis is on monitoring overall network traffic and detecting potential threats that may traverse multiple hosts. NIDS are positioned at strategic points within the network infrastructure, allowing them to analyze and identify suspicious patterns or behaviors across a broader scope. This makes NIDS well-suited for large-scale networks where a centralized approach to intrusion detection is more efficient. On the other hand, HIDS is more appropriate when the focus is on individual host-level security. HIDS is installed on specific devices, monitoring activities at the host level, making it effective for detecting anomalies or attacks targeted at a particular system. The choice between NIDS and HIDS often involves a consideration of the network architecture, the level of granularity required for monitoring, and the specific security goals of the organization.

3. Name 3 major drawbacks of a NIDS?


    1. Limited Visibility:

        One major drawback of a Network-based Intrusion Detection System (NIDS) is its limited visibility into encrypted traffic. As more communication over networks becomes encrypted for security reasons, NIDS may struggle to inspect the contents of encrypted packets. This limitation can hinder the detection of certain types of threats or malicious activities hidden within encrypted communication.

    2. False Positives and Negatives:

        NIDS are prone to generating false positives (incorrectly identifying normal traffic as malicious) and false negatives (failing to detect actual security incidents). Fine-tuning NIDS to distinguish between normal and malicious behavior can be challenging, leading to the risk of either overwhelming security teams with false alerts or missing actual threats.

    3. Network Overhead and Performance Impact:

        Deploying NIDS can introduce network overhead and potentially impact the performance of the monitored network. The process of analyzing and inspecting network traffic in real-time can consume significant resources, affecting the overall network throughput. This performance impact is a concern, especially in high-traffic environments, where the NIDS must efficiently handle large volumes of data without causing delays or disruptions in network operations.

## Analogy


An Intrusion Detection System (IDS) and Intrusion Prevention System (IPS) can be likened to vigilant security guards in a museum. The IDS acts as an observant guard who monitors the visitors and artifacts, keenly watching for any unusual behavior or signs of potential threats. When the IDS detects something suspicious, it raises an alert, much like the guard notifying others about a possible security issue. On the other hand, the IPS takes a more proactive role – it not only detects suspicious activity but also intervenes immediately to prevent any harm. It's akin to a guard equipped with the authority to intervene and stop a potential theft or vandalism, ensuring the security of the museum. Together, these systems work to safeguard the network, much like diligent guards protecting a valuable collection.

## what I want to know more about?
- Gain practical experience by setting up and configuring IDS/IPS solutions in a lab environment.
- how threat intelligence feeds can enhance the capabilities of IDS/IPS by providing real-time information on emerging threats.
## Sources:
- https://blog.rapid7.com/2017/01/11/the-pros-cons-of-intrusion-detection-systems/
- https://www.youtube.com/watch?v=hEgWPWIuq_s&ab_channel=ProfessorMesser
- https://chat.openai.com/
