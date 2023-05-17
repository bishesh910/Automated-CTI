# Bee.Tools ![Bash Automation](https://img.shields.io/badge/Automation-CTI-green)

NOTE: ONLY WORKS ON DEBIAN (FOR NOW)

A Simple Tool for checking malicious IPs from Custom IP list with Virus Total.




## Author

- [@bishesh910](https://www.github.com/bishesh910)


## Installation

Change the file ./Bee.Automated and ./src/ipchecker to executable
```bash
   chmod +x Bee.Automated
```

1. Configure Your Virus Total API key in the 'config.ini' file.

2. Set the threshold level. 

File format something like this.
```bash
[Virustotal]
key = VIRUSTOTAL_API_KEY
lvl = 3

#Configuration for AbuseIPDB (The lvl denotes confidence score and the days denotes maxAgeindays)
[AbuseIPDB]
key = ABUSEIPDB_API_KEY
lvl = 20
days = 90

#Coniguration for MISP (The key denotes the authorization key for the user and event_id is set to null for first time usage. event_id will be rewritten after the script is ran.)
#Example for url(url = https://192.168.1.1/)
[MISP]
url = MISP_URL
key = MISP_AUTH_KEY
event_id = null
```
Run your command by:
```bash
  ./Bee.Automated
```
## Acknowledgements

 - [Srijan Kafle](https://www.github.com/srijankafle)

## What's New? (v1.3)
- Now has "Option for package manager update".
- Formatting style can now be picked on user's choice.
- Provides much cleaner output.
- Now has the function to separate malicious and clean IPs.
- Able to define Severity level on config.ini to justify malicious and clean IP. [works on how many engines found it malicious].
- Integrated AbuseIPDB
- Now automatically takes only unique IPs from list.
- With smart technology now able to determine malicious,clean and IPs you need to review.
- Customisation in your hand : Now you have the power to define the confidence and malicious threshold in Abuse and Virus Total respectively.
- Able to define the number of days for AbuseIPDB in the configuration file.
- Integrated MISP for pushing Malicious IPs.
- Also takes one single IP instead of custom list.
- Automatically creates new event for MISP and appends malicious IPs while avoiding duplication.
- Option to push IPs to MISP.
