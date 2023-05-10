# Topic 1

## Research checklist

> [Link to PDF](./Readings/independent-research-checklist.pdf)

**Relevant**

- [ ] Check the relevance by reading the overview, abstract and/or introduction.
- [ ] Do you think the information will match your needs?

**Objective**

- [ ] Do the writers state their position on the issue in the overview, abstract and/or introduction?
- [ ] Do they use emotive language?
- [ ] Do they have vested interests?

**Research methods**

- [ ] Is it clear how the data was collected?
- [ ] Were the methods appropriate?
- [ ] Do you trust them?

**Current**

- [ ] Is the information up to date?

## Reading

[Ethics in Information Security](./Readings/Ethics%20in%20Information%20Security.pdf)

## Learning objectives

- Understand the central goals and aspects of computer security
- Understand and explain the differences between a range of malware types
- Be able to identify key examples of malware and their historical significance

## What is Computer Security

> Protecting computer related assets against an attacker or threat, as well as ensuring the secure usage of computer hardware and software by non attacker.

### Goals

1. **Prevention**: safeguarding assets from threats
2. **Protection**: having systems to tell you the attack or malicious activity is or about to take place
3. **Reaction**: defining the procedures that enable you to deal with an attack

### Aspects

1. **Policy**: deals with confidentiality, integrity, and availability of data
2. **Threat model**: the set of assumptions about the people involved in malicious activity
3. **Mechanism**: the software or hardware that's designed and implemented to make sure the policies enforced using assumptions we made with the threat model

### Terms

- **Attack**: activities harmful to computer systems, data, software and hardware, etc
- **Risk**: the possibility of damage or loss of digital assets in case of an attack
- **Zero-day vulnerability**: a vulnerability used by an attacker before being discovered by the developer of the software.
  - **zero-day**: the length of time the developer has to react to this particular issue (non at all)
- **Exploit**: the software used to take advantage of a bug or vulnerability
- **Hacker**:
  - **white hats**: aka. Ethical Hackers. Try to find (and fix) weaknesses in the computer or network system with proper permission from a company
  - **black hats**: Try to penetrate the system to gain unauthorized access. (harm, steal)
  - **gray hats**: working with varying combinations of good and bad intentions.

## Types of malicious software

> **Malware**: a peace of software designed to disrupt, damage, and distroy the normal functionality of an information system.

- **viruses**: sharing key characteristics with their biological counterparts.They self-replicate by inserting themselves into other files, programs, documents, etc. Easily spread through dodgy emails, USB sticks, and downloads from untrustworthy sources.

  - _creeper_: one of the first computer viruses (1971)

- **worms**: can replicate itself without attaching to any existing software.

  - _stuxnet_: one of the most destructive worms

- **adware**: displays advertisements on your screen, one of the most visible form of malware, purpose is to collect user's data.

  - _viable_: a well-known adware, infected almost 250 million computers/devices in 2017

- **Trojans**: (named after the famous ancient Greek tale) hide themselves inside an application or program data and spread based on specific user action.

  - _Trojan Zeus_ had infected 1 million user accounts and compromised thousands of FTP, email and bank accounts belonging to large enterprises (2010)

- **Spyware**: spy on the target machine or user, collects information and send it back to the hacker for further use or for sale on the dark web

  - _dark hotel spyware_: use hotel WiFi to target the personal systems of government officials, business typcoons and political leaders

- **keyloggers**: records every keystroke.

  - _Olympic Vision_: launch business email compromise or BEC attacks on businessman in the US, Middle East, and Asia.

- **Ransomware**: victim data is encrypted, backup files are deleted, and demand money for decription.

  - _WannaCry_: Exploited vulnerabilities in older Windows systems (2017 May)

- **Botnets**: computers connecting to the internet are infected without the user realizing, a distributed denial of service attack (DDoS attack) will be launched, where a website/web service collapsed when flooded with too many information.

  - _Ecobot_: used to exploit over 50 known vulnerbilities, infects a wide range of IoT connected devices.

- **rookits**: remain hidden on the target computer and activate in secret. Giving cybercriminals remote access, stealing confidential information, launch the previously mentioned attacks etc.
  - _Zacinlo rootkit_: downloaded within a fake VPN app, opens a browser and interact with it like a human, the browser will open the back door to the comprimise system, which the hacker can then launch attacks.

## Malware analysis and techniques

> Malware analysis is a set of proccesses and techniques that help a security address understand the functionality, origin, impact, and intend to malicious software.
>
> The goal is to find the **IOC** (_Indicator of Compromise_) that depicts the behavior of malicious software. IOCs are also used to develop signatures of malware.

### Static Malware Analysis

- The executable files are examined without running them
- Clean or not, functionality, signatures (a set of distinguishing features used to recognize malware)

#### Scanning

> Running a file through a range of different antivirus softwares

- Ex. virusTotal

#### Hashing

> Running a file through a special piece of software that uses algorithms to produce a code known as a hash., which acts as a digital fingerprint for the file.
>
> An infected version of a file will producea hash that's different from a clean file.

- Ex. Message-Digest Algorithm 5 (MD5), Secure Hash Algorithm 1 (SHA1)

### Dynamic Malware Analysis (aka Behavioral Analysis)

> Execute the malware in the controlled isolated environment (sandbox) to find the IOC.

Ex. (Windows) Process monitor (aka Procmon)

#### Sandbox

> A **sandbox** is a way to dissect and analyze malicious software in a safe and controlled environment.

##### Agent-Based

> Requires software to be installed on every computer monitored.

- Ex. cuckoo, threat expert, bit blase, Comodo

##### Agent-Less

> Monitors computers on the network from afar without installing on every device.

- Ex. VMRay, Analyzer, SNDBOX

Some research suggests Agent-Less are more efficient than Agent-Based sandboxes.

## Ethics

- Ethics are important in computer security because there are wider content ramifications that can have a ripple effect on people and systems.
- Computer scientists, data scientists, programmers, and software engineers may experience security issues and vulnerabilities on a daily basis and need to know how to deal with them.
- Responsible disclosure is subjective and can have legal ramifications.
- We have to consider who is affected by an exploit or vulnerability and decide who to tell and how to communicate the information.
- Large corporations may institute bug bounties, which are incentives for people to find bugs in their system.
- Most security researchers sit somewhere in the periphery of responsible disclosure, wanting to let companies know about the problem and the users about the program.

## Passwords

- Designing secure systems is difficult and perfect security is impossible.
- Data leaks are becoming more common and can be a means for making money.
- There is a market for buying leaked data and zero-day exploits.
- Reusing passwords is a common problem in computer security.
- If one service gets compromised and a user's password is reused across multiple services, then every other service that user uses could potentially be compromised.
- Systems should be designed with rules and functions that allow users to store passwords in a secure way that they can remember.
- Sometimes, people need to be protected from themselves.

## Social Engineering

- Securing systems involves considering human factors
- Social engineering is a common type of attack that exploits people's trust
- Privileged access should be scalable and controlled, and people should have access to information they need only
- USB drive attacks involve leaving drives in public areas for people to pick up and plug into their systems, which can compromise the system
- USB drives can be used as human interface devices to run malicious programs on the system
