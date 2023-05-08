
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

1. Configure Your Virus Total API key in the 'config.ini' file.

2. Set the threshold level. 

File format something like this.
```bash
[API]
key = YOUR_VT_API_KEY

[SEVERITY]
#By default it is set to 3. Set it to your choice.
lvl = 3
```
Run your command by:
```bash
  ./Bee.Automated
```
## Acknowledgements

 - [Srijan Kafle](https://www.github.com/srijankafle)

## What's New? (v1.1)
- Now has "Option for package manager update".
- Formatting style can now be picked on user's choice.
- Provides much cleaner output.
- Now has the function to separate malicious and clean IPs.
- Able to define Severity level on config.ini to justify malicious and clean IP. [works on how many engines found it malicious].
