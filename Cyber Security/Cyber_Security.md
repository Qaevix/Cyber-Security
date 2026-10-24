# What is Cyber Security?

  Cyber security is the practice of protecting computers, networks, systems and data from unauthorized access, attacks, damage or theft.
It includes technologies, processes and security practices used to defend digital systems against threaths such as malware, phishing, ransomware, 
data breaches and hacking attempts.

  The main goal of cyber security is to protect to confidentiality, integrity and availability of information. These three principles are known as the CIA Triad 
and form foundation of information security. Cyber security is used in many areas, including network security, web security, cloud security, penetration testing,
digital forensics, malware analysis and incident response.

## 1. The CIA Triad (Information Security)

It's the foundation model for thinking about security. Every security control you meet usually protects one or more of these three properties.

**Confidentiality** means information is seen only by people who are aloowed to see it.

- **Threats:** Eavesdropping, stolen passwords, data leaks, phishing.
- **Protections:** Encryption (AES, TLS/HTTPS), strong authentication (passwords plus two-factor), access control (user roles and permissions), and the "least privilege"
principle, where people get only the access they need.

**Integrity** means data is accurate, complete and not modified without authorization. It covers accidental changes (a bug, a disk error) as well as malicious ones.

- **Threats:** Tampering with data in transit, SQL injection that alters records, malware, human error.
- **Protections:** Hash functions (SHA-256) to detect changes, digital signatures, checksums, version control, input validation and audit logs that record whı changed what.

**Availability** means systems and data can be used when they're needed.

- **Threats:** DDoS attacks, ransomware, hardware failure, power outages, natural disasters
- **Protectiions:** Backups, redundant servers, load balancing, failover systems, regular updates and disaster recovery plans.

  **Why the triad matters:** the three goals often pıll against each other. Very strict confidentiality (many locks and checks) can reduce availability, because legitimate
  users struggle to get in. Security design is about balancing them of patient records, while a secret military document puts confidentiality first.

  **Programming example:** a login system for a student portal.

  - **Confidentiality** Passwords are stored as salted hashes and the connection uses HTTPS.
  - **Integrity:** Grades can only be changed by teachers and every change is logged.
  - **Availability:** The server is backed up and can handle many students logging in at once.
 
  Some people extend the triad with authenticity and non-repudiation (someone can't deny they performed an action),
  but the three core ideas are the standard.

##  2. The CIA (Central Intelligence Agency)

  Background: The CIA was created by the National Security Act of 1947, after World War II and the intelligence failures around Pearl Harbor.
  It replaced thr wartime OSS (Office of Strategic Services) and became the main civillian foreign intelligence agency of the United States.
  It is headquarters are in Langley, Virginia.

What is does:

- **Collection:** Gathers intelligence from human sources (spies and informants), open sources, and technical means, often working alongside other agencies like the NASA.
- **Analysis:** Turns raw information into assessments for the President and policymakers, such as the daily intelligence briefing.
- **Covert action:** Carries out secret operations to influence events abroad, only when authorized by the President.
- **Counterintelligence:** Protects agains foreign spies and intelligence operations.

**Structure:** It's led by the Director of the CIA and has several directorates, including analysis, operations, science and technology and support. 
It's one part of the larger US Intelligence Community, which has about 18 agencies

**Limits:** By law, the CIA focuses on foreign intelligence and has no police or domestic law enforcement power. That's the main difference from the FBI,
which handles domestic investigations.

**Controversies and history:** It's record is debated. Well-known episodes include the 1953 coup in Iran, the failed Bay of Pigs invasion in Cuba (1961),
the Cold War operations in many countries, the "enhanced interrogation" program after 9/11, and the intelligence failures around Iraq's weapons claims in 2003.
Congressional oversight, such as the Church Committee in the 1970s, was created partly in response to abuses.


  









