# Case 01 - FTP server on printer (Sharp MX-M502N)

## Overview
During passive reconnaissance activities, an FTP server hosted directly on a Sharp MX-M502N multifunction printer at UNI-Milano was discovered as publicly accessible from the Internet. The service allowed anonymous connections and exposed internal functionalities without proper authentication measures.

## Technical Details
- **IP Address**: [Hidden for ethical disclosure]
- **University**: UNI-Milano
- **Device**: Sharp MX-M502N (Multifunction Printer)
- **Service Exposed**: FTP (TCP/21)
- **Authentication**: No authentication required
- **Anonymous Access**: Disabled (but FTP service still exposed publicly)

## Risks
- Unauthorized access to internal document processing functions.
- Potential information leakage (internal scan data, system logs, maintenance reports).
- Possible entry point for lateral movement inside the university network.
- Exposure to known vulnerabilities associated with embedded printer FTP servers.

## Severity
**Critical**

## Notes
While the FTP service did not allow anonymous login, its public exposure remains a serious risk factor, especially considering the nature of the device and its potential links to internal infrastructure.

## Recommendation
- Immediately restrict FTP access to internal university networks (private VLAN or VPN).
- Implement firewall rules to block external traffic to TCP/21.
- Regularly update printer firmware and monitor for unauthorized access attempts.
- Consider disabling the FTP feature entirely if not strictly necessary.
