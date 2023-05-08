# Bee.Tools ![Bash Automation](https://img.shields.io/badge/Automation-CTI-green)

NOTE: ONLY WORKS ON DEBIAN (FOR NOW)

A Simple Tool for checking malicious IP from Custom IP list with Virus Total.




## Author

- [@bishesh910](https://www.github.com/bishesh910)


## Installation

Change the file ./Bee.Automated and ./src/ipchecker to executable
```bash
   chmod +x Bee.Automated 
   chmod +x src/ipchecker
```

1. Configure Your Virus Total and AbuseIPDB API key in the 'config.ini' file.

2. Set the threshold level for Virustotal malicious count and abuseIPDB confidence score

3. Set The maxAgeInDays. 

File format something like this.
```bash
[VT_API]
key = YOUR_VT_API_KEY_HERE

[Abuse_API]
key = YOUR_ABUSE_API_KEY_HERE


#VT Severity (by default Set to 3)
[VT_SEVERITY]
lvl = 3

#Abuse Severity (by default set to 20%)
[Abuse_SEVERITY]
lvl = 20


#Time (Should be between 1-365)
[Abuse_maxAgeInDays]
days = 90
```
Run your command by:
```bash
  ./Bee.Automated
```
## Acknowledgements

 - [Srijan Kafle](https://www.github.com/srijankafle)

## What's New? (v1.2)
- Integrated AbuseIPDB
- Now automatically takes only unique IPs from list.
- With smart technology now able to determine malicious,clean and IPs you need to review.
- Customisation in your hand : Now you have the power to define the confidence and malicious threshold in Abuse and Virus Total respectively.
- Able to define the number of days for AbuseIPDB in the configuration file.
