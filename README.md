# Network Device Logging and Analytics
A way to find the adversary in your network devices

## Overview
Network devices are end points too. That's why I mapped the MITRE ATT&CK Enterprise Tactics and Techniques to the network devices and their operating systems. I hope the MITRE ATT&CK team incorporates these changes in. Additionally, there are simple Sigma rules to aide in detection.

## MITRE ATT&CK Model
Out of the current 244 Enterprise ATT&CK Techniques, I believe that 64 of them can apply to Network Devices as endpoints to be exploited. They are listed in the MITRE folder, along with a JSON file of the Techniques from ATT&CK Navigator.

In the technique overview file, each one is listed, with what data source you may need, the example commands, and a brief comment on why it's applicable.

### Proposed Changes to MITRE ATT&CK Enterprise Model


## Sigma Rules
In the rules directory are ## rules that map back to MITRE ATT&CK Techniques. They are all written in Sigma format to be SIEM agnostic. They are all based on the assumption that you currently, or will, collect AAA logs from your network devices - specifically the "Accounting" logs.

## AAA Logging References
