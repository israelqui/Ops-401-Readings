# Reading 2
# Cloud Security Principles and Frameworks
## Why is this topic important?

Understanding cloud security principles and frameworks in tech is crucial because it underpins the foundation of trust and reliability in modern digital systems. With businesses and individuals increasingly relying on cloud services, a robust grasp of security principles ensures the protection of sensitive data, applications, and infrastructure from a myriad of potential threats, including cyber attacks, data breaches, and compliance violations. Mastery of these concepts empowers tech professionals to implement robust security measures, adhere to industry standards, fortify defenses against evolving threats, and ultimately safeguard the integrity, confidentiality, and availability of critical information, fostering a resilient and secure digital ecosystem.

1. Explain the levels of abstraction in AWS to someone without a technical background.


Imagine AWS as a colossal digital toolbox with various layers. At the top level, you have services like Amazon EC2, which are like fully assembled tools ready for use, such as a pre-built computer. Going deeper, there's a middle layer providing broader functionalities, akin to a collection of parts forming a tool, like AWS Lambda, which lets you create custom functions without worrying about the underlying infrastructure. At the base, you have the raw materials and infrastructure, the fundamental building blocks—these are like the basic elements needed to construct any tool, similar to AWS's storage services or networking components. Each level offers different levels of control and complexity, catering to various needs without requiring users to start from scratch.

2. What are the control plane and data plane responsible for in container abstraction?


In container abstraction, the control plane and data plane serve distinct roles. The control plane manages the overall orchestration and configuration of containers. It handles tasks like scheduling containers onto specific nodes, ensuring resource allocation, maintaining desired state, and managing scaling or updates. Essentially, it's responsible for the high-level decisions about where containers run and how they interact.


On the other hand, the data plane is focused on the actual data flow and processing within the containers themselves. It deals with the forwarding of network traffic to and from containers, applying necessary policies or transformations, and handling data-related operations within the containers. The data plane ensures that data is correctly routed and processed within the containerized environment, managing the runtime behavior of containers in terms of handling incoming and outgoing data traffic.

3. Where does AWS Lambda fall in the layers of abstraction and what makes it so special?


AWS Lambda sits at a higher level of abstraction within AWS services. It belongs to the category of serverless computing, which abstracts away the underlying infrastructure entirely, allowing developers to focus solely on writing code and executing functions without managing servers.

Lambda operates in the middle layer of abstraction. It's like a tool that lets you create custom functions without worrying about the underlying infrastructure. You provide the code, and Lambda takes care of scaling, provisioning, and managing the resources needed to run that code. This abstraction enables developers to focus on writing efficient code, without the overhead of managing servers, allowing for quick development, scalability, and cost-effectiveness. Lambda's "pay-per-use" pricing model, where you only pay for the compute time your code consumes, is also one of its defining features, making it appealing for various use cases, from small applications to large-scale systems.

## Things i want to know more about:
- Understand the division of security responsibilities between the cloud service provider (CSP) and the customer.
- Explore encryption mechanisms for data at rest and data in transit. This includes understanding techniques like encryption key management,
- Familiarize with compliance standards (such as GDPR, HIPAA, SOC 2) and the governance frameworks (like NIST, CIS Benchmarks) applicable to an industry.

# Sources:
- https://aws.amazon.com/blogs/architecture/compute-abstractions-on-aws-a-visual-story/
- https://www.horangi.com/blog/13-compliance-frameworks-for-cloud-based-organizations
- https://cloudsecurityalliance.org/
- https://cloudsecurityalliance.org/research/cloud-controls-matrix/
- https://cloudsecurityalliance.org/research/guidance/
- https://chat.openai.com/
