# Network Device Logging and Analytics
A way to find the adversary in your network devices

## Overview
Network devices are end points too.  These are simple Sigma rules to aide in detection using Syslog and AAA logs to find adversary using techniques while on a router or switch.  This research is specific to Cisco devices, but the theory is easily expanded to other vendors.  

## MITRE ATT&CK Model
MITRE ATT&CK now has a Network Device Enterprise Matrix to map how an adversary may exploit network devices.  However, there are many Techniques in ther other Enterprise matrices that are not listed as Network platform, but are very easily accomlished on a network device. 

## Sigma Rules
In the rules directory are 13 rules that map back to 37 MITRE ATT&CK Techniques. They are all written in Sigma format to be SIEM agnostic. They are all based on the assumption that you currently, or will, collect Syslog and AAA logs from your network devices - specifically the "Accounting" logs.

## AAA Logging References
To read more about TACACS and RADIUS see this [resource](https://tacacs.net/docs/TACACS_Advantages.pdf).

## References
* Thanks to Florian and his Sigma project https://github.com/Neo23x0/sigma
* Thanks to the ATT&CK Team at MITRE https://github.com/mitre-attack