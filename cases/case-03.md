# Case 03 - OpenStack Dashboard exposed (Padova)

## Overview
An OpenStack Dashboard management interface was discovered publicly accessible on the Internet, linked to UNI-Padova. The dashboard allows administrative management of cloud computing resources, making its exposure particularly sensitive.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Padova
- **Service Exposed**: OpenStack Dashboard (Horizon interface)
- **Authentication**: Login portal publicly available without network restrictions

## Risks
- Brute-force attacks against login credentials.
- Exposure of internal cloud management resources (VMs, storage, networking).
- Potential for full administrative compromise if credentials are weak or leaked.
- Risk of privilege escalation and lateral movement within academic cloud environments.

## Severity
**High**

## Notes
The exposure of cloud management panels is particularly critical, as it may allow attackers to create, modify, or destroy virtualized resources belonging to the university.

## Recommendation
- Restrict access to the OpenStack Dashboard to internal trusted networks only.
- Enforce strong password policies and two-factor authentication (2FA) for all users.
- Regularly monitor authentication attempts and implement brute-force protection mechanisms.
- Consider moving the dashboard behind a VPN or bastion host.
