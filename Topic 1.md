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

We work with software on a daily basis. As such, we may be exposed to security issues and vulnerabilities as we work. It's a bit like being a driver a high-speed, you recognize it as a degree of risk. But you understand that risk and you know how to deal with them.

You may have seen the term **responsible disclosure** used in the literature that you've engaged with. There is some subjectivity about what this means in real terms and there can be legal ramifications too.

- Who's affected if there's an exploit available in a system?
- What does that mean in real terms to human beings, to people who are using those systems?
- What if this is a system that's in common usage, other people might suffer from the same vulnerability.

If we find some exploit mechanism in our system that we weren't aware of before. It may be the case that somebody's already leveraged this in some way, and we haven't seen the activity.

- Who do we have a responsibility to in this context, in terms of disclosing this issue and telling people about what's actually happening?

Should we tell everybody, should we tell nobody? We have to make a decision about who to tell and how to tell them.

Large corporations may encourage this behavior, they may will give you some money if you find a bug in their system. They may very closed down in that context and they may get very upset that you've exploited something in the system, even if it's a widely-known exploit.

Most security researcher sits somewhere in the periphery in this term. So they want to let the companies know that there's a problem. They want to let the users know that their program, but then might be in terms of that problem bit of push and pull.

- Who do I tell first?

If I told the user, somebody else might exploit it. If I tell the company, they may get upset about it or they may take legal action.

We also have to think about security in a distributed way. It's not just enough in terms of thinking about how you perceive things, but how other people perceive things in the world. Most of us now rely on cloud based services to deliver content and offer on demand computing. These systems are located all over the world and you might not even know where the server that you're using is located. We have to think about, well, if that information is somewhere else, can I guarantee it's security? Can I guarantee it's safety? If I have a server hosted somewhere else, I have to think about the legal ramifications of the data being stored on that server.

## Passwords

I'm going to talk about how a particular exploitation might manifest and how it might cause problems later down the line.

Designing truly secure systems is actually really, really hard work and we can't design anything that's perfectly secure. Given that most computational power is what we rely on to encode data then eventually there will come a time in which these powerful algorithms that we look at now, in the future, are no longer powerful enough to secure our systems.

One of the most prolific leaks, they utilized an encryption technique wherein the same encryption key was used and the password had a one-to-one mapping. Every time a particular password was encoded, the encoded version always look the same and there was always a one-to-one mapping.

With most good cryptography, it's all about pushing it in that one direction, it should be easy to encode but very, very difficult to decode. In this case, it means that the encrypted version always equates to the same thing. Let's look at why this might be a problem. Some people also used hints and the hints were stored in the database, in some cases, some of the hints were easy to figure out. It might be the case that one person has put a hint in there that's quite cryptic and very difficult to work out without knowing the person but if they share the same password as somebody else and they have put a hint in there that's easy to figure out that mapping goes both ways.

Reusing passwords is a common problem in computer security and you're often advised not to reuse passwords and different services just in case one of them gets compromised.

You have to be very careful in providing rules and functions that make sense to people that allow them to store passwords in a way in which they can understand and remember them but also they are secure and for their own benefit. You sometimes have to protect people from themselves. We can design systems to be more secure but these things also have implications. If we ask people to use longer passwords or passwords that are more difficult to guess, they might struggle to remember those passwords and, in those cases, we might also see security breaches come from that.

A good system design has to balance accessibility with security and usability. We have to keep all of these things in mind when we're designing systems that are to be secure.

## Social Engineering

- What does security infrastructure breaches look like
- What are the manifestation of these attacks?
- How are they launched?
- How do people go about solving these issues when a system has been compromised in some way?

Social engineering is actually one of the most common types of attack hackers, and it doesn't rely on technical manifestations of attacks. Not all staff in their company or necessarily trained to the same level of skills as some of us might be accustomed to.

Now let's take a scenario, I find a USB drive on the floor, looks like somebody's lost this drive, or maybe it's one of my colleagues, or one of my friends who've lost their important data, of course, I don't want to leave it where somebody might find it, I don't want to leave that information somewhere, it might be pictures that are on there or other sensitive data relating to the business but I've got no way of identifying what that USB driver is and what's on it. I have to make a decision straight away and have to decide, well, what am I going to do? The quickest way to find out what's on the USB drive is to plug it into my system, now that might be problematic.

Now let's take another example of this, we're all very technical and we all come across these things regularly and most of us at this point in time have enough training to know not to do these things and to know to be wary of these things. But what about if a police officer stops your industry and asked to see some identification? What do you do? In most cases, people would probably comply. Given that this is a figure of authority, you'd say, yes, I am who I am, there's my driver's license, there's my ID. But in this case, this is a scenario where you could have a similar example, you could have a person trying to get access to your information who isn't who they say they are and most of us probably wouldn't be able to look at a police ID and recognize whether or not that's authentic.

