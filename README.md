# Cybersecurity-CTF-Labs-Collection-Insecure-Deserialization-XML-Race-Conditions
A curated, searchable index of hands-on CTF labs covering Java, Python, Node.js, PHP, Ruby, and .NET insecure deserialization, gadget chains, XXE, DTD injection, and race condition basics from Learn SecByte.
# Insecure Deserialization, XML Injection & Race Conditions CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on language-specific insecure deserialization (Java, Python, PHP, Ruby, Node.js, .NET), gadget chain exploitation to Remote Code Execution (RCE), XML parser abuses (XPath, XML Bomb, DTD injection), and race condition fundamentals hosted on Learn SecByte.

This repository is designed for application security engineers, penetration testers, CTF competitors, security researchers, and developers aiming to master object serialization risks and complex data-parser vulnerabilities.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [Insecure Deserialization & Gadget Chains (Multi-Language)](#insecure-deserialization--gadget-chains-multi-language)
  - [XML Parser Abuses & Injection Attacks](#xml-parser-abuses--injection-attacks)
  - [Concurrency & Race Condition Fundamentals](#concurrency--race-condition-fundamentals)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Insecure deserialization occurs when untrusted data is used to populate an object, enabling attackers to alter logic, hijack execution flow, or execute arbitrary code via gadget chains. Paired with complex data parser vulnerabilities like XML Entity Expansion and XPath Injection, these flaws represent high-impact risks in enterprise software architectures.

This repository organizes hands-on cybersecurity labs from Learn SecByte into logical, multi-language learning paths covering modern application security vulnerabilities.

---

## Lab Collection & Index

| Lab Title | Language / Technology | Primary Vulnerability | Access Link |
| :--- | :--- | :--- | :--- |
| **Race Condition Basics** | Web / Systems | Concurrency & Race Flaws | [Access Lab](https://learn.secbyte.org/ctf/race-condition-basics) |
| **Deserialization to RCE** | Cross-Language | Insecure Deserialization RCE | [Access Lab](https://learn.secbyte.org/ctf/deserialization-to-rce) |
| **Gadget Chains Deserialization** | Cross-Language | Advanced Gadget Chains | [Access Lab](https://learn.secbyte.org/ctf/gadget-chains-deserialization-to-rce) |
| **Ruby Marshal Abuse** | Ruby | Marshal Deserialization | [Access Lab](https://learn.secbyte.org/ctf/ruby-marshal-abuse-deserialization-to-rce) |
| **Node.js Deserialization** | Node.js / JavaScript | Safe Deserialization Patterns | [Access Lab](https://learn.secbyte.org/ctf/nodejs-deserialization-from-gadget-chains-to-safe-patterns) |
| **Python Pickle Injection** | Python | Pickle RCE | [Access Lab](https://learn.secbyte.org/ctf/python-pickle-injection-deserialization-to-rce) |
| **.NET Deserialization** | .NET / C# | BinaryFormatter / Gadgets | [Access Lab](https://learn.secbyte.org/ctf/dotnet-deserialization-gadget-chains-detection) |
| **PHP Object Injection** | PHP | Unsafe `unserialize()` | [Access Lab](https://learn.secbyte.org/ctf/php-object-injection-unsafe-deserialization) |
| **Java Deserialization** | Java | ObjectInputStream / Defenses | [Access Lab](https://learn.secbyte.org/ctf/java-deserialization-from-gadget-chains-to-safe-defenses) |
| **XPath Injection** | XML / Web | Query Injection & Exfiltration | [Access Lab](https://learn.secbyte.org/ctf/xpath-injection-from-xml-queries-to-data-exfiltration) |
| **XML Bomb (Billion Laughs)** | XML | Entity Expansion DoS | [Access Lab](https://learn.secbyte.org/ctf/xml-bomb-entity-expansion-parser-abuse) |
| **DTD Injection** | XML / XXE | Blind Out-of-Band Exfiltration | [Access Lab](https://learn.secbyte.org/ctf/dtd-injection-from-dtd-basics-to-blind-exfiltration) |

---

## Categories

### Insecure Deserialization & Gadget Chains (Multi-Language)
Hands-on CTF labs exploring object serialization, magical method invocation, and payload construction across major ecosystems:

* **Deserialization to RCE Fundamentals:** Understanding object stream parsing and arbitrary code execution paths.
  * Lab Link: https://learn.secbyte.org/ctf/deserialization-to-rce
* **Gadget Chains Construction:** Building execution chains from existing class libraries to reach dangerous sinks.
  * Lab Link: https://learn.secbyte.org/ctf/gadget-chains-deserialization-to-rce
* **Java Deserialization Defenses:** Exploiting Java `ObjectInputStream` gadget chains and implementing safe look-ahead object filters.
  * Lab Link: https://learn.secbyte.org/ctf/java-deserialization-from-gadget-chains-to-safe-defenses
* **Python Pickle Injection:** Crafting malicious `__reduce__` methods in Python `pickle` payloads to execute shell code.
  * Lab Link: https://learn.secbyte.org/ctf/python-pickle-injection-deserialization-to-rce
* **PHP Object Injection:** Triggering `__wakeup()`, `__destruct()`, and `__toString()` magic methods through unsafe `unserialize()`.
  * Lab Link: https://learn.secbyte.org/ctf/php-object-injection-unsafe-deserialization
* **Ruby Marshal Abuse:** Exploiting Ruby's `Marshal.load` to trigger gadget chains resulting in remote code execution.
  * Lab Link: https://learn.secbyte.org/ctf/ruby-marshal-abuse-deserialization-to-rce
* **Node.js Deserialization:** Analyzing vulnerable JavaScript serialization packages (e.g., `node-serialize`) and implementing safe JSON patterns.
  * Lab Link: https://learn.secbyte.org/ctf/nodejs-deserialization-from-gadget-chains-to-safe-patterns
* **.NET Deserialization Detection:** Identifying unsafe .NET formatters (e.g., `BinaryFormatter`, `NetDataContractSerializer`) and auditing gadget chains.
  * Lab Link: https://learn.secbyte.org/ctf/dotnet-deserialization-gadget-chains-detection

### XML Parser Abuses & Injection Attacks
Practical security labs covering structured document parsing, entity expansion attacks, and out-of-band data exfiltration:

* **XPath Injection:** Manipulating XML path expressions to bypass authentication and exfiltrate internal XML databases.
  * Lab Link: https://learn.secbyte.org/ctf/xpath-injection-from-xml-queries-to-data-exfiltration
* **XML Bomb (Billion Laughs Attack):** Abusing recursive Document Type Definition (DTD) entity expansion to cause Denial of Service (DoS).
  * Lab Link: https://learn.secbyte.org/ctf/xml-bomb-entity-expansion-parser-abuse
* **DTD Injection & Blind Exfiltration:** Constructing external DTDs for blind XML External Entity (XXE) data exfiltration over HTTP/FTP.
  * Lab Link: https://learn.secbyte.org/ctf/dtd-injection-from-dtd-basics-to-blind-exfiltration

### Concurrency & Race Condition Fundamentals
Entry-level security labs focused on thread synchronization, asynchronous state handling, and race condition basics:

* **Race Condition Basics:** Fundamentals of shared memory state, non-atomic checks, and basic concurrency flaws.
  * Lab Link: https://learn.secbyte.org/ctf/race-condition-basics

---

## Learning Path

Follow this structured learning path to master deserialization, XML security, and concurrency:

1. **Concurrency Core Concepts**
   - Study race condition basics to understand shared state and asynchronous execution timing.
2. **XML Security & Parser Exploitation**
   - Practice XPath queries manipulation and XML entity expansion (XML Bomb).
   - Advance to external DTD injections for out-of-band data exfiltration.
3. **Insecure Deserialization Fundamentals**
   - Master object serialization theory and magic method behavior in PHP and Python.
4. **Advanced Multi-Language Gadget Chains**
   - Analyze complex gadget chains across Java, .NET, Ruby, and Node.js.
   - Implement defensive practices including serialization filters and safe data formats (e.g., JSON/Protobuf).

---

## How to Use the Labs

1. Select a lab from the collection index or category breakdown above.
2. Launch the interactive practice scenario directly on Learn SecByte.
3. Complete the hands-on objectives covering static code analysis, payload crafting, and exploitation.
4. Review safe code patterns and filter configurations to solidify software security knowledge.

---

## Disclaimer

This repository is strictly intended for educational research, authorized security testing, and defensive training. All concepts, payloads, and lab environments are provided to help developers and security practitioners secure modern applications. Performing unauthorized attacks against external systems or services without explicit written permission is strictly prohibited.
