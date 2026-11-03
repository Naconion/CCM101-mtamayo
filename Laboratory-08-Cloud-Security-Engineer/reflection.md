# Mission 8 Reflection

## **Host-Based Firewall Protection**

A host-based firewall sits right on the operating system level of a single machine. Even if someone manages to bypass the outer network perimeter or router, this firewall acts as a solid last line of defense. It checks every incoming packet against strict local rules, which helps block attackers from moving laterally across internal cloud networks.

**Importance of Port Management**

Managing open ports is huge when it comes to shrinking your attack surface. Every open port with a running service is basically an open door for exploits, zero-day vulnerabilities, or brute-force attacks. Closing down everything you don't actively need makes it way harder for automated port scanners to find a way in.

**Dangers of Public Database Exposure**

Leaving a database port (like MySQL on port 3306) wide open to the public internet is a massive security risk. It practically invites automated SQL injection, credential stuffing, and data theft. In a real-world enterprise setting, databases should always live in isolated internal subnets where only authorized app servers or secure VPNs can reach them.

**Perspective shift on Server Vulnerability**

Doing this lab really opened my eyes to how fast exposed cloud servers get targeted. If you spin up a server and leave the default settings alone without a firewall, it's vulnerable almost instantly. It really hammered home why you have to lock things down *before* pushing any live workloads out.

**GitHub Portfolio Growth**

Wrapping up this eighth mission feels awesome. Looking at my GitHub Cloud Computing Portfolio now, it's cool to see how much practical experience I've built up—everything from deploying cloud infrastructure and managing Linux servers to handling container orchestration, monitoring, and now network security.
