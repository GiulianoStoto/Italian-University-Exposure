# Case 06 - FTP services exposed without anonymous login (Padova)

## Overview
During passive reconnaissance, an FTP service associated with UNI-Padova was found to be publicly accessible over the Internet. Although anonymous login was disabled, the mere exposure of an FTP server remains a risk without additional authentication controls.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Padova
- **Service Exposed**: FTP (TCP/21)
- **Authentication**: Username and password required (no anonymous access)

## Risks
- Credential bruteforce attempts against the FTP login.
- Potential compromise of user accounts if weak credentials are used.
- Opportunity for reconnaissance and mapping of the internal directory structure.
- Possible exploitation of unpatched FTP server vulnerabilities.

## Severity
**Medium**

## Notes
While anonymous login is disabled, public exposure of FTP services without IP filtering or VPN restriction still presents a risk, particularly against automated attack tools.

## Recommendation
- Limit FTP access to trusted IP addresses through firewall rules.
- Enforce strong password policies for all FTP users.
- Monitor login attempts and enable account lockout mechanisms after multiple failures.
- Consider transitioning to more secure alternatives such as SFTP or FTPS.
