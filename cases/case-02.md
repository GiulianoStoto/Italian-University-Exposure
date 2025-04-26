# Case 02 - FTP server with anonymous access (ProFTPD)

## Overview
During passive reconnaissance, an FTP server at UNI-Verona was discovered allowing **anonymous access** without authentication. The server was publicly reachable from the Internet and exposed critical FTP functionalities.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Verona
- **Service Exposed**: FTP (TCP/21) - ProFTPD server
- **Authentication**: Anonymous access allowed (no credentials needed)

## Risks
- Full anonymous access to potential sensitive directories and files.
- Risk of exfiltration or tampering with university resources.
- Possible platform for hosting malicious files (risk of blacklisting the university's IP).
- Potential foothold for lateral movement into internal networks.

## Severity
**High**

## Notes
Anonymous access dramatically increases the risk profile of FTP servers, particularly when publicly exposed without strict directory or access controls.

## Recommendation
- Immediately disable anonymous FTP access.
- Restrict FTP access to internal users only via firewall ACLs.
- Regularly audit and monitor FTP services for unauthorized access or uploads.
- Consider migrating file sharing services to more secure protocols (e.g., SFTP, HTTPS).
