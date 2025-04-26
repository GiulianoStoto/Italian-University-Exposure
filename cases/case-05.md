# Case 05 - Legacy Apache/SSL server (Centro ANTARES - Bologna)

## Overview
Passive reconnaissance identified an old Apache web server exposed by Centro ANTARES (University of Bologna) with outdated SSL/TLS protocols enabled. This server could be a weak link within the larger university network due to its obsolete configuration.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Bologna
- **Service Exposed**: Apache HTTP Server
- **Server Version**: Apache 2.2.x (End-of-Life)
- **SSL/TLS Protocols**: Support for deprecated TLS 1.0 and 1.1 detected

## Risks
- Exposure to well-known vulnerabilities affecting outdated Apache versions.
- Weak encryption allows the possibility of MITM (Man-In-The-Middle) attacks.
- Potential for information disclosure through poorly secured services.
- Increased likelihood of successful exploitation due to publicly available exploits for Apache 2.2.x.

## Severity
**Medium**

## Notes
While no immediate access was gained, the presence of outdated web server software represents a significant technical debt and security liability for the institution.

## Recommendation
- Upgrade the Apache server to a supported, modern version (2.4.x or higher).
- Disable deprecated SSL/TLS protocols and enforce TLS 1.2 or TLS 1.3 only.
- Conduct a full review of server configurations and patch all known vulnerabilities.
- Implement regular maintenance schedules to prevent future obsolescence.
