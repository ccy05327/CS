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

- ([Original Source](https://ieeexplore.ieee.org/document/6152082)) [K. S. Wilson, Conflicts Among the Pillars of Information Assurance](./Readings/Conflicts%20Among%20the%20Pillars%20of%20Information%20Assurance.pdf)
    [Markdown ver.](/Readings/Conflicts%20Among%20the%20Pillars%20of%20Information%20Assurance.md)

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