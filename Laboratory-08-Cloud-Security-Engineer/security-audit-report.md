# Security Audit Report: Chapter 8 Concepts

### 1. The Principle of Least Privilege (PoLP)
The Principle of Least Privilege dictates that any identity, account, or process should be granted only the minimum access rights and resources strictly necessary to perform its intended job. In cloud user accounts, enforcing PoLP minimizes the potential blast radius if credentials become compromised. By preventing unauthorized privilege escalation, it keeps critical cloud resources isolated from malicious exploitation.

### 2. Attack Surface
The attack surface of a virtual machine encompasses the sum total of all reachable endpoints, listening network ports, active services, and potential vulnerabilities exposed to external actors. A broader attack surface means attackers have more entry vectors to scan, probe, and exploit. Reducing this surface involves disabling unnecessary background daemons and blocking unused network ports.

### 3. Default Deny Policy
A Default Deny policy automatically blocks all inbound network traffic unless it explicitly matches a predetermined whitelist rule. Relying on reactive blocklists is ineffective against dynamic, automated threat actors who constantly cycle IP addresses and search for open vulnerabilities. By denying everything from the outset, the server remains fortified against unauthorized scans, admitting only verified and necessary operational traffic.
