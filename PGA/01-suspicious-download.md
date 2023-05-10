# The suspicious download

## Scenario

It was just a few months ago that you were submitting your thesis as a BSc Computer Scientist, interested in cybersecurity. Since then, you have worked very hard to secure your dream job in a related field. One of your applications was successful and you were invited for a job interview by human resources.

You are now attending the last round of interviews to secure your position as a 'Junior Security Analyst' at 'SafeDreams' – a startup company specialising in cybersecurity consultancy. The interviewer asks you to consider the following situation:

> Jan is conducting research with his favourite browser when, suddenly, the browser crashes. In an attempt to reopen the browser, Jan is prompted with a message requesting a browser update and a file is automatically downloaded on his laptop. The file now sits in the download folder, ready to be executed. Despite the harmless name and file extension, Jan is very suspicious that the file might not be legitimate. He decides to consult the opinion of an expert and arranges an appointment with you to assess the situation.

The interviewer asks you to *write a report* on possible responses to the situation and in particular **identify** and **describe** some key characteristics and exploration of the threat.

## Submission

1. Please describe the file malware’s potential typology and its characteristics, given the scenario. What sort of threat do you think this might pose if the code were to be executed or run on the local machine?

2. Describe three valid methods of analysing the nature and potential risks of the downloaded file without imposing unnecessary risk or compromising the system.

## Report

There are a few key characteristics indicating this file might be malware. Browser crashed, file downloaded without user's consent, and the seemingly harmless file name and extension.

If the file were to be executed, it could pose a significant threat. It might be designed to steal personal information, such as passwords, credit card numbers, or other sensitive data. It could also be designed to damage or disrupt the system, such as deleting files or causing the computer to crash. The malware could also be a backdoor for other malicous software to be installed on the user's system.

1. Scan the file with an online malware detector from a legitimate company in the cybersecurity fields.
2. Run the file in a sandbox environment to monitor its behaviour so that it doesn't affect the local machine.
3. Consult a cybersecurity expert to analyse the file and provide a detailed report on any potential threats or risks.

### ChatGPT

#### Question 1

Based on the scenario provided, the downloaded file is suspicious, and it may potentially be a type of malware. Malware is an umbrella term that includes a variety of malicious software designed to cause harm to computer systems and networks. Malware can take many forms, including viruses, Trojans, worms, ransomware, spyware, and adware.

Without analyzing the file, it is impossible to know with certainty what type of malware it might be. However, some of the characteristics that might indicate that the file is malware are:

- The file was automatically downloaded without Jan's consent, which suggests that it may have been delivered through a phishing email, social engineering tactics, or a drive-by download.

- The file has a harmless name and file extension, which might be an attempt to disguise the true nature of the file and make it seem harmless.

- The browser crashed before the file was downloaded, which could indicate that the malware exploited a vulnerability in the browser or a plugin.

If the file were to be executed or run on the local machine, it could pose a significant threat. Some possible consequences of running the malware include:

- Theft of sensitive information: The malware might be designed to steal personal or confidential information from the user's computer, such as login credentials, banking information, or other sensitive data.

- Installation of additional malware: The malware might act as a backdoor to allow other malware to be installed on the user's computer, leading to further compromise.

- Ransomware attack: The malware might encrypt the user's files and demand a ransom in exchange for the decryption key, which can be extremely disruptive and costly.

- System disruption or damage: The malware might be designed to delete files, modify system settings, or cause other damage to the user's computer, leading to loss of productivity or significant repair costs.

In conclusion, given the characteristics and potential consequences described above, it is crucial to handle suspicious files with care, and in this case, advise Jan not to execute or run the downloaded file without further analysis or professional support.

#### Question 2

When analysing a suspicious file, it is crucial to do so without putting the system at risk or compromising its integrity. Here are three valid methods of analysing the nature and potential risks of the downloaded file:

1. Use an online malware scanner: Online malware scanners are available from reputable cybersecurity companies and can be used to scan the downloaded file for malware. These scanners utilise signature-based detection, behaviour analysis, or machine learning algorithms to identify malware, and they can provide a quick and straightforward way to determine whether the file is malicious or not. However, the user should ensure that the online scanner is legitimate and secure and does not pose any risk to the system.

2. Conduct a sandbox analysis: A sandbox analysis involves running the downloaded file in a virtual environment or sandbox, which isolates the file from the system and monitors its behaviour. Sandboxing can help identify any malicious activities, such as attempts to connect to external servers or make changes to system files. This method is useful for identifying new or unknown types of malware, but it requires technical expertise to set up and may not always be foolproof.

3. Consult a cybersecurity expert: Consulting a cybersecurity expert or a reputable security firm is an effective way to analyse the file's nature and potential risks. The expert can examine the file, conduct a thorough analysis, and provide a detailed report on any potential threats or risks. They can also provide advice on how to handle the file and any necessary actions that need to be taken to mitigate the risk of infection or damage to the system. This method ensures a high level of accuracy and reliability, but it may involve additional costs and time.

In conclusion, when analysing a suspicious file, it is essential to use a safe and secure method that minimises the risk of infection or damage to the system. Utilising an online malware scanner, conducting a sandbox analysis or consulting a cybersecurity expert are all valid methods that can help identify any potential risks and provide guidance on how to handle the file.
