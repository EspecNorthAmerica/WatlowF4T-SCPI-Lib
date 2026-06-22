# WatlowF4T SCPI Library

A Python 3 built-in library using the Standard Commands Programming Instrumentation (SCPI) was implemented to communicate, control and operate Watlow F4T for this application.

Communication protocol for this applications is available only via TCP/IP using port 5025 implemented by Watlow. The sample program included in this implementation provides a starting point. Users interested in a full SCPI implementation can expand 

## Disclaimer

Copyright (c) 2026 ESPEC North America, Inc.

This library is provided free of charge for communicating with Watlow F4T
controllers using SCPI over TCP/IP. It is provided "as is", without warranty of
any kind, express or implied.

Users are responsible for testing and validating this software in their own
environment before using it with any equipment or process. The authors and
contributors are not liable for damages, losses, equipment issues, process
interruptions, or other consequences resulting from the use or misuse of this
software.

# Requirements

## F4T Software Version 

The SCPI protocol for Watlow F4T is application with new firmware on F4T unit. According to Watlow F4T software (tested on 04:07:0012). It also only applies in TCP/IP protocol application, using port 5025. IT does not support serial itnerface.  

## Python 3 version 

This library makes use of the built-in Python Library. It requires importing the register/unregister. 

Thus, only the standard install of Python 3 is required. This library has been tested on the following Python 3 versions: 
 
 - Python 3.6
 - Python 3.8
 - Python 3.9
 - Python 3.13 

Since the above versions (up to 3.9) already reached their end of life (EOL), current versions of Python 3 are recommended. 

# Installation

This implementation was originally written for GNU/Linux, but it can be used Mac OS and MS Windows platform, provided the necessary requirements and packages of Python 3 are met. To install Python 3 on MS Windows, simply navigate to the [www.python.org](http://www.python.org), download the package for Windows. 

### Python 3 on GNU/Linux

The complete install of Debian and AlmaLinux, or Ubuntu GNU/Linux should include Python 3 standard install that includes the SCPI library. If Python 3 is not already installed, the following commands can be issued in the respective GNU/Linux platform: 

* Debian/Ubuntu: ```sudo apt install python3```
* AlmaLinux: ```sudo dnf install python3``` 

Note: On AlmaLinux or Debian GNU/Linux platform, the sudo command refers to issuing the above command as root. 

# How to Use this F4T SCPI library

## Installing & Configuring F4TSCPI library

There are two ways to use this distribution:

1. PyPI
2. src folder

However, neither the PyPI package nor the src distribution folder has been published.

Until a packaged release is available, the easiest way to use this free library is to clone the repository to your local system and check out the main branch.

## Cloning the F4TSCPI repo

Clone this free library to your local system as follows:

```git clone git@github.com:EspecNorthAmerica/WatlowF4T-SCPI-Lib.git```

```git checkout main```

## Testing

This implementation has been tested on various Watlow F4T with different configurations according to their installed modules for: 

- Temp with cascade
- Temp and Humi single staged refrig
- Temp with single state refrig
- Temp and Humi with cascade refrig

To run the program to control and operate your Watlow F4T, issue: 

* MS Windows: ```python f4t_run.py```
* GNU/Linux: ```sudo python3 f4t_run.py``` 

## Implementation 

For required application not implemented in the sample run program may be added by referencing the SCPI commands in the spread fould in the folder: f4t+scpi_cmds 
