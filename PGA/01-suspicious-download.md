# The suspicious download

## Scenario

It was just a few months ago that you were submitting your thesis as a BSc Computer Scientist, interested in cybersecurity. Since then, you have worked very hard to secure your dream job in a related field. One of your applications was successful and you were invited for a job interview by human resources.

You are now attending the last round of interviews to secure your position as a 'Junior Security Analyst' at 'SafeDreams' – a startup company specialising in cybersecurity consultancy. The interviewer asks you to consider the following situation:

    Jan is conducting research with his favourite browser when, suddenly, the browser crashes. In an attempt to reopen the browser, Jan is prompted with a message requesting a browser update and a file is automatically downloaded on his laptop. The file now sits in the download folder, ready to be executed. Despite the harmless name and file extension, Jan is very suspicious that the file might not be legitimate. He decides to consult the opinion of an expert and arranges an appointment with you to assess the situation.

The interviewer asks you to *write a report* on possible responses to the situation and in particular **identify** and **describe** some key characteristics and exploration of the threat.

## Report

The first step can be to check the file with a static malware like `virusTotal`, running the file with different antivirus softwares. 

If the result still gives you some doubt, you can then try to run a hashing algorithm through it, this will give you a more thorough analysis by comparing the hash to other hashes in the database which contains clean files. If your file results in a different hash than the other files, the file is malicious. 

Lastly if you were still suspicious about the file, we can run some dynamic malware analysis for you. This will require either installing the required software on your device, or giving us internet access to monitor your device. We will be running the file on a safe and isolated environment so that everyone's device is protected and try to find the IOC (Indicator of Compromise) in the file. 