# Network Device Logging and Analytics
A way to find the adversary in your network devices

## Overview
Network devices are end points too. That's why I mapped the [MITRE ATT&CK Enterprise Tactics and Techniques](https://attack.mitre.org/tactics/enterprise/) to the network devices and their operating systems. I hope the MITRE ATT&CK team incorporates these changes. Additionally, there are simple Sigma rules to aide in detection.

## MITRE ATT&CK Model
Out of the current 244 Enterprise ATT&CK [Techniques](https://attack.mitre.org/techniques/enterprise/), I believe that 64 of them can apply to Network Devices as endpoints to be exploited. They are listed in the [MITRE folder](mitre_attack), along with a [JSON file](mitre_attack/Network_Device_Techniques.json) of the Techniques from [ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/enterprise/).

In the [mitre_attack/README.MD](mitre_attack/README.md) file, each one is listed, with what data source you may need, the example commands, and a brief comment on why it's applicable.

### Proposed Changes to MITRE ATT&CK Enterprise Model
1. It's my opinion that "Network Devices" be added as an additional Platform to the Enterprise technology area
2. Network Device Logs should be expanded and redefined:
    * Network Device logs - Specifically refers to Syslog from the device
    * Accounting, Authentication, Authorization (AAA) - referring to remote logging from TACACS+/RADIUS
3. That the Techniques that are applicable to Network Devices get updated to reflect that

## Sigma Rules
In the rules directory are 12 rules that map back to MITRE ATT&CK Techniques. They are all written in Sigma format to be SIEM agnostic. They are all based on the assumption that you currently, or will, collect AAA logs from your network devices - specifically the "Accounting" logs.

## AAA Logging References
To read more about TACACS and RADIUS see this [resource](https://tacacs.net/docs/TACACS_Advantages.pdf).

## References
* Thanks to Florian and his Sigma project https://github.com/Neo23x0/sigma
* Thanks to the ATT&CK Team at MITRE https://github.com/mitre-attack