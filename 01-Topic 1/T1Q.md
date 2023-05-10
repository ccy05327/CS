# Topic 1 Quiz

## Lesson 2 Security threats

### The basics

1. The three main aspects of Computer Security are:

   - [ ] Software, Hardware and Defence
   - [ ] Policy, Confidentiality and Integrity
   - [x] Policy, Threat Model and Mechanism
   - [ ] Attack, Risk and Hacking

    <br>

    > Yes. 'Policy' deals with how we make decisions about security, 'Threat Model' concerns how we make judgments about the threats posed to our system, and 'Mechanism' is how we go about executing those assumptions and decisions.

2. Hackers are individuals that:

    - [x] Try to break into a computer network without permission, but not always to steal data or damage the target.
    - [x] Try to break into a computer network without permission, and with the intension of stealing data and damaging the target.
    - [x] Try to find weaknesses in a computer network with permission from the target company.

### Malware

1. How do worms differ from viruses?

    - [] Worms can 'burrow' deeper into the computer system to avoid detection, but viruses cannot.

    - [] Viruses are usually harmless, and worms can cause far more damage than viruses.

    - [x] Worms can replicate themselves, without needing to be attached to existing files or software.

    - [] Worms can only affect Programmable Logic Controllers (PLCs), whereas viruses have a broader range of targets.
2. Adware...

    - [x] Displays adverts during web browsing and collects data on user activity. This is sometimes legitimate, but usually it is not, and done  without the permission of the user.

    - [] Attaches itself to files in your computer system, showing unwanted advertisements and messages when you view your documents. 

    - [] Displays adverts during web browsing. This is done with the knowledge of the user and is usually harmless.

### Botnets and rootkits

1. Which of the following are true of a 'botnet'?

    - [x] <span style="color: salmon">The use of a command and control (C&C) server to give orders to compromised computers.</span>

        > True. A compromised computer that has become part of the 'robot network' awaits orders from a server that is controlled by the attacker.

    - [ ] Files are encrypted and backup files are deleted.

    - [ ] Key presses are monitored and sent back to a central server for processing.

    - [x] Can be used to launch a Distributed Denial of Service (DDOS) attack.

        > True. The large number of computers that can be infected and connected together means they can easily flood target web services with requests and information to force them to overload and fail.

2. What characteristics make botnets and rootkits particularly dangerous forms of malware?

    - [ ] They corrupt files and delete backup files, asking for a fee to be paid in bitcoin for files to be restored.

    - [ ] They can cause the host computer to fail and crash unexpectedly.

    - [x] They stay hidden, are incredibly difficult to detect and can execute their mission without the victim computer/user knowing they are there.

        > Correct. This difficulty in detection leaves the computer open to misuse over a long period of time by the attacker.

## Lesson 3 Malware analysis

### Malware analysis

1. The two types of malware analysis are:

    - [x] Static

    - [ ] Botnet

    - [ ] Hashing

    - [x] Dynamic

    - [ ] Virus

2. How can 'hashing' be used to detect infected files during static analysis?

    - [ ] The suspect file is scanned using anti-virus software. This produces a hash. The hash is compared to examples in a database. If the hash matches an entry in the database, the file is infected.

    - <span style="color:mediumPurple">[ ] A hashing algorithm, such as MD5, is run against a suspect file. This hash (unique string) is compared to that of a clean file. If they are the same, then the suspect file is infected.

    - <span style="color:salmon">[ ] Strings from a clean file and a suspect file are compared. If they are different then they are run through a hashing algorithm. If they are different, then the suspect file is infected.</span>

    - [x] A hashing algorithm, such as MD5, is run against a suspect file. A check against a known database of bad hashes will help to find if a file is malicious

### Keep safe

1. Dynamic Analysis is useful because...

    - <span style="color:salmon">[ ] It allows a security professional to work out how much damage the malware could potentially do.</span>

    - [x] It allows a security professional to detect malware that can evade static analysis.

    - <span style="color:salmon">[ ] It allows a security professional to determine the signature of the malware, so it can be identified later.</span>

    - [x] It allows a security professional to discover the functionality of the malware.

2. Do you have up-to-date anti-virus protection on your computer at home or at work? If not, why not? Has the material you've covered in this topic made you think any differently about your security software on your devices at all? How?

    - No, simply because they usually cost money and I don't really understand the differences when choosing one. 








