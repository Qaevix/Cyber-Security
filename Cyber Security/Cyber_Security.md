
# 🛡️ What Is Cybersecurity?

````markdown
**Cybersecurity** is the practice of protecting computers, networks, applications and data from unauthorized access, misuse,
disruption, damage or theft. It combines **people, processes and technology** to reduce security risks and respond to incidents.

Common threats include malware, phishing, ransomware and data breaches. Cybersecurity covers areas such as network security,
application security, cloud security, penetration testing, digital forensics, malware analysis and incident response.

Its central goals are to preserve the **confidentiality, integrity and availability** of information. Together, these principles
form the **CIA Triad**, a foundational model in information security.

> In information security, CIA stands for Confidentiality, Integrity and Availability.
````

## 1. The CIA Triad

````markdown
  The CIA Triad helps us understand what needs protection and choose appropriate security measures. A single measure can support
more than one principle.

| Principle | Purpose | Key Question |
|-----------|---------|--------------|
| **Confidentiality** | Prevent unauthorized disclosure | Who can access the information? |
| **Integrity** | Protect against improper changes | Can we trust the information? |
| **Availability** | Maintain timely and reliable access | Can we use it when needed? |

### Confidentiality

**Confidentiality** ensures that information is accessible only to authorized people, systems or processes.

#### Common Threats

- Eavesdropping on network communications
- Stolen passwords and compromised accounts
- Phishing and social engineering
- Accidental exposure of sensitive files
- Misconfigured access permissions

#### Typical Protections

- **Encryption:** Protect stored data with suitable encryption and network traffic with TLS, as used by HTTPS.
- **Multi-factor authentication (MFA):** Require different types of proof of identity, such as a password and a security key.
- **Access controls:** Define which resources each user or system may access.
- **Least privilege:** Grant only the permissions needed to perform a task.

> **Example:** A student can view their own academic records but cannot access another student's private information.

### Integrity

**Integrity** protects information against unauthorized or improper modification or destruction. It helps preserve the accuracy
and completeness of data. Integrity addresses deliberate tampering as well as accidental changes caused by software bugs, hardware
faults or human error.

#### Common Threats

- Unauthorized changes to database records
- SQL injection that modifies or deletes data
- Tampering with files or network messages
- Accidental edits and data corruption

#### Typical Protections

- **Cryptographic hashes:** Detect changes by comparing a file's hash with a trusted reference value.
- **Message authentication codes and digital signatures:** Help verify integrity and authenticity.
- **Authorization controls:** Restrict who can create, modify or delete information.
- **Input validation:** Check that submitted data meets the application's requirements.
- **Parameterized queries:** Separate SQL instructions from supplied values to prevent SQL injection.
- **Version control and protected audit logs:** Track changes and support investigation and recovery.

> **Important:** A hash alone does not guarantee authenticity. If an attacker can replace both a file and its reference hash,
the comparison will not reveal the tampering. Ordinary checksums help detect accidental corruption but are not designed to resist
malicious changes.

> **Example:** Only authorized teaching staff can change a student's grade, and every change is recorded in a protected audit log.

### Availability

**Availability** ensures that authorized users can access systems, services and information when needed.

It involves keeping services operational and restoring them within an acceptable time after a failure or attack.

#### Common Threats

- Distributed denial-of-service (DDoS) attacks
- Ransomware
- Hardware failures
- Power outages and network disruptions
- Natural disasters

#### Typical Protections

- **Backups and tested recovery procedures:** Restore information after loss or corruption.
- **Redundancy and failover:** Keep services operating when a component fails.
- **Load balancing and capacity planning:** Handle expected traffic and periods of high demand.
- **Monitoring and maintenance:** Detect problems and reduce avoidable disruptions.
- **Disaster recovery plans:** Define how critical services will be restored.

> **Important:** Backups support recovery, but they do not automatically keep a service online. Availability also depends
on resilient infrastructure and tested restoration procedures.

> **Example:** A university portal remains accessible during registration, even when many students log in at once.
````

## 2. Why the CIA Triad Matters

````markdown
  Security decisions often involve trade-offs. Strict access controls may protect sensitive information, but poorly designed
authentication can also prevent legitimate users from accessing essential services.

The right balance depends on the system's purpose. A hospital, for example, needs patient records to remain confidential and
accurate while being available to authorized medical staff during emergencies.

| Incident | Primary Principle Affected |
|----------|----------------------------|
| Private student records are leaked | Confidentiality |
| A grade is changed without authorization | Integrity |
| The student portal goes offline during registration | Availability |

> One incident can affect multiple principles. Ransomware can make information unavailable, modify files and expose stolen data.
````

## 3. Practical Example: A Student Portal

````markdown
A student portal demonstrates how the three principles work together.

### Protecting Confidentiality

- Use **HTTPS** to protect network traffic.
- Check permissions before returning private information.
- Store passwords using a dedicated password-hashing method with a unique salt.
- Require multi-factor authentication where appropriate.

### Preserving Integrity

- Verify permissions on the backend before accepting grade changes.
- Use parameterized database queries.
- Validate submitted data.
- Maintain protected audit logs recording who changed a grade and when.

### Maintaining Availability

- Monitor service health and respond to failures.
- Plan capacity for busy registration periods.
- Use redundant components to reduce interruptions.
- Maintain backups and regularly test recovery procedures.
````

## 4. Beyond the CIA Triad

````markdown
Other security concepts complement the three core principles:

| Concept | Meaning |
|---------|---------|
| **Authenticity** | Confidence that an entity or piece of information is genuine |
| **Accountability** | The ability to trace actions to the responsible entity |
| **Non-repudiation** | Evidence supporting the origin or performance of an action that helps counter a later denial |

````










