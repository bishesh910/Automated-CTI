# Bee.Tools ![Bash Automation](https://img.shields.io/badge/Automation-CTI-green)

NOTE: ONLY WORKS ON DEBIAN (FOR NOW)

A Simple Tool for checking malicious IP from Custom IP list with Virus Total.




## Author

- [@bishesh910](https://www.github.com/bishesh910)


## Installation

Change the file ./Bee.Automated and ./src/bee to executable
```bash
   chmod +x Bee.Automated 
   chmod +x src/bee
```

1. Configure Your Virus Total API key in the 'config.ini' file.

File format something like this.
```bash
[API]
key = YOUR_VT_API_KEY_HERE
```
Run your command by:
```bash
  ./Bee.Automated
```

## Acknowledgements

 - [Srijan Kafle](https://www.github.com/srijankafle)
