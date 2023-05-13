# Topic 2 Quiz

## Network security objectives

1. The main objectives of network security are:

   - [ ] Ingenuity

   - [ ] Accountability

   - [ ] Isolation

   - [x] Integrity

   - [x] Confidentiality

   - [ ] Deployability

   - [x] Availability

   - [ ] Transparency

## DOS and flooding

1. Which of the following is the correct definition for a DOS attack?

   - [ ] <span style="color:salmon"> A DOS (Denial of Service) attack is one where the target server is convinced that all requests are bad, and so gives up, shuts down and denies users of its services. </span>

   - [ ] A DOS (Denial of System) attack is one where the target network will not acknowledge other components of the host system due to overload and stress.

   - [ ] A DOS (Distribution of Service) attack is one where the traffic of a specific server is redistributed to several other servers under the attacker's control.

   - [x] A DOS (Denial of Service) attack is one where legitimate users of a service are prevented from accessing the system resources that they need.

2. What is a SYN flood attack?

   - [x] An attack that exploits the TCP/IP handshake process by flooding the target server with SYN requests from invalid or spoofed IP addresses, resulting in increased server load and increased response time to legitimate users.

   - [ ] An attack where oversized ping packets are sent to the target server.

   - [ ] An attack where the target server is forced to try and synchronise it's internal clock with hundreds of others round the world at the same time, resulting in confusion and failure.

## The Internet of (bad) things

1. Why is it important to pay attention to security in Internet of Things (IoT) devices?

   - [x] Each IoT device can potentially become part of a botnet to launch a DDOS.

   - [ ] IoT devices are inherently insecure.

   - [ ] IoT devices could join together to create a super AI.

   - [x] There will be thousands more of these devices than there are desktops and laptops.

   - [x] Many of these devices are made cheaply and so manufacturers are not concerned with patching them.

2. What are the core modules of the Mirai botnet software?

   - [x] Bot, Server, Loader.

   - [ ] <span style="color: salmon">Attack, Kill, Scan</span>

     > No. These are the functions of the bot module.

   - [ ] Bot, Hunter, Killer.

   - [ ] Scout, Recruiter, Commander, Messenger.

## Wireless networking standards

1. Wireless networks are newer and, therefore, more secure than wired networks.

   - [x] FALSE
     > Correct. There are more access points, more ways to intercept any data transmitted, all without the added inconvenience of needing access to the wired network within a building.
   - [ ] TRUE

2. What is the single best way to protect yourself from wireless hacking?

   - [ ] Strong encryption (using WEP).

   - [ ] Use a strong password generator.

   - [ ] Change your login details frequently.

   - [x] Strong encryption (using WPA2).
     > Correct. WEP is weak enough to be broken in under five minutes and no longer provides much protection in the modern-age of wireless telecommunications. Use WPA2 as a minimum instead.

## Firewall revision

1. What type of firewalls were featured in the previous lecture?

   - [x] Proxy

     > Yes. This sits at the boundary between the LAN and anything outside it – as a WAN and the internet. As such, it acts as a kind of gatekeeper to the LAN from outside.

   - [x] Stateful

     > Yes. This is where the firewall can see the packets in context of what came before, and so make more sophisticated decisions than a stateless firewall.

   - [ ] Cloud

   - [ ] Software

   - [ ] Brick

   - [x] Stateless

     > Yes. This is a firewall that simply applies a set of rules to each packet that crosses a certain point in the network.

## Intrusion detection systems (IDS)

1. Why do intrusion detection systems evolve hand-in-hand with machine learning and AI algorithms?

   - [ ] Because the machine learning can generate large amounts of data to test an IDS.

   - [ ] Because machine learning software is better than hardware.

   - [x] Because machine learning, AI and IDSs revolve around the ability to recognise patterns in data.
     > Yes. The focus of machine learning is on pattern recognition, and an IDS needs to recognise normal and abnormal patterns in the network data it is watching over.
   - [ ] Because better machine learning makes IDSs cheaper.
