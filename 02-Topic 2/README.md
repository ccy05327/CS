# Topic 2 Network Security

## Learning Objectvives

- Describe the CIA objectives of network security
- Use real examples to describe how DoS attacks and DDoS attacks work including those using botnets
- Describe the levels of security in wireless networks and common attacks vectors

## Objectives of Network Security (CIA)

Network security is a set of policies and practices that protect a network, consisting of plans/rules and practical tasks.

1. **Confidentiality**- Controlling access to files on the network, limiting read access for users based on their authorization.

2. **Integrity**- Controlling the ability to change things on the network and its contents over time, by defining what people can do with files, folders and servers.

3. **Availability**- Ensuring the network is accessible, balancing high security measures with the need for access, and guarding against extreme measures that could limit accessibility to an impractical degree.

### Reading

- ([Original Source](https://ieeexplore.ieee.org/document/6152082)) [K. S. Wilson, Conflicts Among the Pillars of Information Assurance](./Readings/Conflicts%20Among%20the%20Pillars%20of%20Information%20Assurance.pdf), [Markdown ver.](/Readings/Conflicts%20Among%20the%20Pillars%20of%20Information%20Assurance.md)

    > **Summary**
    > Interactions between the five pillars of information assurance (availability, integrity, authentication, confidentiality, and nonrepudiation) can cause conflicts. Efforts to advance one pillar can interfere with another. Availability can conflict with confidentiality, integrity, and authentication. Confidentiality and integrity are facets of controlled information access. Understanding these conflicts can help identify situations where mitigation of one type of risk might increase another. Proposed measures should be analyzed to determine whether risk trade-offs are acceptable.

## Types of Attacks

- **Denial of Service (DOS) attack**: denies service to a network by overloading or taking down a network service
- **Attack surface**: network layer model (7-layer) where attacks take place
- Relevant layers:
  - Hardware: physical network components
  - Data link: defines addresses on the network, ARP (Address Resolution Protocol) flood attack
  - Network: sends basic data on the network
  - Transport: negotiates connections with other machines on the network and breaks up data into packets
  - Presentation
  - Application
- Examples of DOS attack types:
  - ARP flood attack: sends a flood of requests on the network, the machine responds to each request, overloading the machine's resources.
  - Other attacks can target different layers of the network model.

## The anatomy of a DDOS, botnets and Mirai

- DDoS attacks aim to take down a service or website by flooding it with requests.
- Denial of Service (DoS) attack is a similar attack but involves only one machine.
- Botnets are networks of infected devices used to carry out DDoS attacks.
- Botnets are controlled by a central server that sends them instructions to attack.
- Botnets can have millions of devices and use normal communication channels like Internet Relay Chat to receive instructions.
- The Internet of Things (IoT) devices pose a new threat as they are often not well protected or updated, making them easy targets for botnet attacks.
- IoT devices include a wide range of devices, such as refrigerators, doorbells, and security cameras.
- The case study of the Mirai botnet shows how a real botnet operates
    > ... the most prominent Mirai DDoS attact was on DNW provider Dyn, resulting in inaccessibility of serveral high-profile websites such as GitHub, Twitter, Reddit, Netflix and many others. After analysis, Dyn estimated that there were up to 100,000 malicious endpoints involved in the attact

## Wireless attacts: WiFi attact vectors

- The Wifi Alliance is an organization of companies producing wireless technology, which aims to ensure compatibility between wireless devices.
- The history of wireless network protocols and security is briefly discussed, focusing on major hardware iterations of wireless standards, such as 802.11a and 802.11b.
- Four different attacks on wireless networks are described.
The lecture advises that an understanding of cryptography is necessary to fully comprehend the attacks and recommends reading on the subject.
- Security protocols within wireless standards are also discussed, including the ill-fated WEP and later WPA, WPA2, and WPA3.
- The lecture provides personal experience with wireless networks and experimenting with different network speeds and video codecs.
- Manufacturers may release firmware updates to upgrade previous devices to support newer standards or security protocols

## Readings

**Classic paper reporting on WEP’s vulnerabilities**

Scott R. Fluhrer, Itsik Mantin, and Adi Shamir. 2001. [Weaknesses in the Key Scheduling Algorithm of RC4](https://dl.acm.org/doi/10.5555/646557.694759). In Revised Papers from the 8th Annual International Workshop on Selected Areas in Cryptography (SAC '01). Springer-Verlag, Berlin, Heidelberg, 1–24.

**This is a good (if a bit old) article about attack vectors for different Wifi protocols such as WEP, WPA and LEAP:**

([PDF](/Readings/WiFi%20attack%20vectors.pdf)) Hal Berghel and Jacob Uecker. 2005. [WiFi attack vectors](https://dl.acm.org/doi/10.1145/1076211.1076229). Commun. ACM 48, 8 (August 2005), 21–28. DOI:<https://doi.org/10.1145/1076211.1076229>
Very thorough review of security in different wireless technologies used in IoT devices:

([PDF](/Readings/Attacks%20and%20Defenses%20in%20Short-Range%20Wireless%20Technologies%20for%20IoT.pdf)) K. Lounis and M. Zulkernine, "[Attacks and Defenses in Short-Range Wireless Technologies for IoT](https://ieeexplore.ieee.org/abstract/document/9090905)," in IEEE Access, vol. 8, pp. 88892-88932, 2020, doi: 10.1109/ACCESS.2020.2993553.


## Learning objectives

- Described three types of firewall and reason about the appropriate type of firewall to use for a given situation
- Explain how Introsion Detection Systems work and give examples of historical and contemporary systems

## Firewalls - our first line of defence

### Stateless Firewall

- aka Access Control Lists (ACL)
- check all traffic passing through & apply rules to each packet
> ACL checks packet characteristics like destination IP address or accessing a specific port to determine if it meets any rules.
- somewhat inefficient (check all traffic individually)

### Stateful Firewall

- remember connections & allow future packets flow freely after initial connection is verified
- more efficient especially in large networks

### Proxy Firewall

- act as intermediaries between the internal network (LAN) and the external network (WAN).
> Machines in the LAN communicate with the proxy firewall, which retrieves data from external sources on their behalf.
- provide enhanced security by isolating the internal network and only exposing the proxy server to external connections.
-  can thoroughly check data for viruses and ensure the internal network's protection.

## Intrusion Detection Systems (IDS)

**Why do we need to detect intrusions?**

> Most security experts agree that a completely secure system is impossible to achieve. So we must stay alert for attacks.
> 
> Kemmerer and Vigna, 2002

**What is the best approach?**

> The model is based on teh hypothesis that exploitation of a system's vulnerabilities involves abnormal use of the system; therefore, security violations could be detected from abnormal patterns of system usage.
>
> Denning, 1987


### Challenges

- Effectiveness: false positives, false negatives
- Performance: resource use, speed
- Ability to operate over a whole network

**Early Systems (1970s-1980s)**: Dorothy Denning was a pioneer in IDS design, developing the concept of abnormal and normal behaviour profiles and detection in the IDES system

**State-of-the-art (2019)** IDS systems now employ deep learning techniques, such as long short-term memory (LSTM) networks, to recognize patterns over time.

IDS **datasets** are used to test and evaluate IDS performance, providing labeled data on network activities.

**Commercial systems** like Cisco and Darktrace offer contrasting approaches to IDS, with Cisco using hardware-based analysis and Darktrace utilizing machine learning and AI.

## Readings

**Dorothy Denning’s classic paper about IDS**

([PDF](/Readings/An%20Intrusion-Detection%20Model.pdf)) D. E. Denning, "[An Intrusion-Detection Model](https://ieeexplore.ieee.org/document/1702202),"

**Overview on Intrusion Detection**

([PDF](/Readings/Intrusion%20detection%20-%20a%20brief%20history%20and%20overview.pdf)) R. A. Kemmerer and G. Vigna, "[Intrusion detection: a brief history and overview](https://ieeexplore.ieee.org/document/1012428),"

**A recent state of the art paper about IDS, using deep networks of course**

([PDF](/Readings/A%20Novel%20Intrusion%20Detector%20Based%20on%20Deep%20Learning%20Hybrid%20Methods.pdf)) S. Wang, C. Xia and T. Wang, "[A Novel Intrusion Detector Based on Deep Learning Hybrid Methods](https://ieeexplore.ieee.org/document/8819467),"

**The NSL-KDD dataset**

https://www.unb.ca/cic/datasets/nsl.html
