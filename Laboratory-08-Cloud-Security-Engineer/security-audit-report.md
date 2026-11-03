# Security Audit Report

## Principle of Least Privilege (PoLP)
The Principle of Least Privilege (PoLP) states that user accounts, processes, and applications should only be granted the minimum necessary access rights and permissions required to perform their specific tasks. In cloud environments, applying PoLP minimizes potential damage by ensuring that a compromised credential cannot be used to access or exploit administrative services and sensitive data across the wider infrastructure.

## Attack Surface
The term "attack surface" refers to the sum total of all vulnerable points, open ports, exposed services, and potential vectors that an unauthorized user or malicious actor could attempt to exploit to gain entry into a virtual machine. Minimizing the attack surface involves disabling unnecessary software services, closing unused network ports, and enforcing strict user access controls.

## Default Deny Policy
A Default Deny policy is a foundational security configuration where all incoming network traffic is blocked automatically unless an explicit rule allows it. This approach is significantly safer than blocking specific malicious IP addresses because automated attacks constantly originate from new, unpredictable sources; denying all unauthorized traffic by default ensures that unknown threats are shielded out instantly.
