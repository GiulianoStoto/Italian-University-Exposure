# Case 04 - OpenStack Dashboard exposed (Pisa)

## Overview
During passive reconnaissance, an OpenStack Dashboard login page was found publicly exposed by UNI-Pisa. The dashboard manages critical cloud resources and its exposure could severely impact the security of the university's internal infrastructure.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Pisa
- **Service Exposed**: OpenStack Dashboard (Horizon interface)
- **Authentication**: Login page publicly accessible over the Internet

## Risks
- Brute-force login attempts targeting user accounts.
- Unauthorized access to virtual machines, storage systems, and networking components.
- Potential to create, modify, or delete critical cloud resources.
- Risk of privilege escalation leading to deeper infiltration of university systems.

## Severity
**High**

## Notes
Although login credentials are required, exposure of management portals significantly increases attack surface and potential compromise vectors.

## Recommendation
- Restrict OpenStack Dashboard access to internal networks (using VPN or firewall rules).
- Enforce strict password and authentication policies, including 2FA.
- Implement monitoring for unusual login attempts and failed authentications.
- Review and limit user permissions according to the principle of least privilege.
