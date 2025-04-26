# Case 08 - SonicWALL web management portals exposed (Pisa)

## Overview
During passive reconnaissance, SonicWALL firewall management interfaces were discovered publicly exposed on UNI-Pisa networks. The interfaces were accessible without IP-based restrictions and presented SSL certificate issues.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Pisa
- **Service Exposed**: SonicWALL Firewall Web Management Interface
- **Authentication**: Login page publicly available
- **SSL Status**: Self-signed or invalid certificates detected

## Risks
- Target for brute-force login attempts.
- Exposure of critical network management tools to Internet-based threats.
- Potential for firewall misconfigurations to be exploited remotely.
- Higher risk of credential phishing or session hijacking due to invalid SSL certificates.

## Severity
**Low**

## Notes
Although authentication is required to access the firewall configuration, exposing firewall management ports to the Internet without VPN restrictions or strong security measures represents a significant risk to network security.

## Recommendation
- Restrict management interface access to trusted internal networks only.
- Enforce strong password policies and multi-factor authentication (MFA).
- Install valid SSL certificates from trusted authorities.
- Regularly monitor and audit access logs for suspicious activities.
