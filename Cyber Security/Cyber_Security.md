

# 🛡️ What Is Cybersecurity?

````markdown
Cybersecurity is the practice of protecting computers, networks, applications and data from unauthorized access, misuse, disruption, damage or theft. It combines **people, processes and technology** to reduce security risks and respond to incidents.

Common threats include malware, phishing, ransomware and data breaches. Cybersecurity covers areas such as:

- Network and application security
- Cloud security
- Penetration testing
- Digital forensics
- Malware analysis
- Incident response

The main goal is to preserve the **confidentiality, integrity and availability** of information. These three principles form the **CIA Triad**, a foundational model in information security.

> **Note:** Here, CIA means **Confidentiality, Integrity and Availability**, not the Central Intelligence Agency.

## 📑 Contents

- [1. The CIA Triad](#1-the-cia-triad)
  - [Confidentiality](#confidentiality)
  - [Integrity](#integrity)
  - [Availability](#availability)
- [2. Why the CIA Triad Matters](#2-why-the-cia-triad-matters)
- [3. Practical Example: A Student Portal](#3-practical-example-a-student-portal)
- [4. Beyond the CIA Triad](#4-beyond-the-cia-triad)

## 1. The CIA Triad

The CIA Triad helps us identify what needs protection and choose appropriate security controls. A single control can support more than one principle.

| Principle | Main purpose | Key question |
|---|---|---|
| **Confidentiality** | Prevent unauthorized disclosure | Who can access the information? |
| **Integrity** | Prevent improper modification or destruction | Can we trust the information? |
| **Availability** | Maintain timely, reliable access | Can we use it when needed? |

### Confidentiality

**Confidentiality** ensures that information is accessible only to authorized people, systems or processes.

#### Common threats

- Eavesdropping on network communications
- Stolen passwords and compromised accounts
- Phishing and social engineering
- Accidental exposure of private files
- Misconfigured access permissions

#### Typical protections

- **Encryption:** Protect stored data with suitable encryption, such as AES, and network traffic with TLS, as used by HTTPS.
- **Multi-factor authentication (MFA):** Require more than one type of proof of identity.
- **Access controls:** Define which resources each user or system may access.
- **Least privilege:** Grant only the permissions required to perform a task.

> **Example:** A student can view their own academic records but cannot access another student's private information.

### Integrity

**Integrity** protects information against unauthorized or improper modification or destruction. It helps keep data accurate and complete throughout its lifecycle.

Integrity addresses both deliberate tampering and accidental changes caused by software bugs, hardware faults or human error.

#### Common threats

- Unauthorized changes to database records
- SQL injection that modifies or deletes data
- Tampering with files or network messages
- Accidental edits and data corruption

#### Typical protections

- **Cryptographic hashes:** Detect changes by comparing a file's hash with a trusted reference value.
- **Message authentication codes and digital signatures:** Help verify integrity and authenticity.
- **Authorization controls:** Restrict who can create, modify or delete information.
- **Input validation:** Check that input meets the application's requirements.
- **Parameterized queries:** Keep SQL instructions separate from supplied values to prevent SQL injection.
- **Version control and protected audit logs:** Track changes and support investigation and recovery.

> **Important:** A hash alone does not prove that data is trustworthy. If an attacker can replace both a file and its reference hash, the comparison will not reveal the tampering. Ordinary checksums help detect accidental corruption but are not designed to resist malicious changes.

> **Example:** Only authorized teaching staff can update a student's grade, and each change is recorded in a protected audit log.

### Availability

**Availability** ensures that authorized users can access systems, services and information when needed.

It involves keeping services operational and restoring them within an acceptable time after a failure or attack.

#### Common threats

- Distributed denial-of-service (DDoS) attacks
- Ransomware
- Hardware failures
- Power outages and network disruptions
- Natural disasters

#### Typical protections

- **Backups and tested recovery procedures:** Restore information after loss or corruption.
- **Redundancy and failover:** Keep services operating when a component fails.
- **Load balancing and capacity planning:** Handle expected traffic and periods of high demand.
- **Monitoring and maintenance:** Detect problems and reduce avoidable disruptions.
- **Disaster recovery plans:** Define how critical services will be restored.

> **Important:** Backups support recovery, but they do not automatically keep a service online. Availability also depends on resilient infrastructure and tested restoration procedures.

> **Example:** A university portal remains accessible during registration, even when many students log in at once.

## 2. Why the CIA Triad Matters

Security decisions often involve trade-offs. A restrictive access policy may protect sensitive information, but a poorly designed authentication process can also block legitimate users.

The right balance depends on the system's purpose. For example, a hospital needs patient records to remain:

- **Confidential:** Accessible only to authorized people.
- **Accurate and protected:** Safe from improper changes.
- **Available:** Accessible to authorized medical staff during emergencies.

The CIA Triad provides a practical way to assess the impact of a security incident:

| Incident | Primary principle affected |
|---|---|
| Private student records are leaked | Confidentiality |
| A grade is changed without authorization | Integrity |
| The student portal goes offline during registration | Availability |

> A single incident can affect multiple principles. Ransomware, for example, can interrupt access, alter files and expose stolen information.

## 3. Practical Example: A Student Portal

A student portal shows how all three principles work together.

### Protecting Confidentiality

- Use **HTTPS** to protect network traffic.
- Check permissions before returning private information.
- Store passwords using a dedicated password-hashing method with a unique salt.
- Require additional authentication where appropriate.

### Preserving Integrity

- Verify permissions on the backend before accepting grade changes.
- Use parameterized queries to prevent SQL injection.
- Validate submitted data.
- Keep protected audit logs recording who changed a grade and when.

### Maintaining Availability

- Monitor service health and respond to failures.
- Plan capacity for busy registration periods.
- Use redundant components to reduce interruptions.
- Maintain backups and regularly test recovery procedures.

## 4. Beyond the CIA Triad

Other security concepts complement the three core principles:

| Concept | Meaning |
|---|---|
| **Authenticity** | Confidence that an entity or piece of information is genuine |
| **Accountability** | The ability to trace actions to the responsible entity |
| **Non-repudiation** | Evidence supporting the origin or performance of an action that helps counter a later denial |

Together, these concepts help guide the design and operation of trustworthy systems.
````



  









