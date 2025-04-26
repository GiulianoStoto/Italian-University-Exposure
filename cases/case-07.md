# Case 07 - Multiple portals under maintenance or construction (Napoli, Ancona, others)

## Overview
Several university subdomains, notably from UNI-Napoli and UNI-Ancona, were found publicly reachable and displaying "Under Construction" or "Maintenance" pages. Although these pages did not expose sensitive data directly, they still represent an unnecessary attack surface.

## Technical Details
- **IP Addresses**: [Hidden for ethical disclosure]
- **Universities**: UNI-Napoli, UNI-Ancona, UNI-L'Orientale
- **Services Exposed**: Apache Web Servers showing maintenance pages
- **Authentication**: No authentication enforced

## Risks
- Discovery of backend technologies through exposed HTTP headers and error messages.
- Enumeration of server versions, frameworks, or CMS used.
- Potential leakage of internal configuration details if maintenance pages are misconfigured.
- Increased visibility to automated scanners and bots.

## Severity
**Low**

## Notes
Although no sensitive content was found during passive analysis, maintenance or construction pages should not be left openly accessible, especially if associated services are in staging or development phases.

## Recommendation
- Restrict access to maintenance or development sites via IP whitelisting.
- Remove staging environments from the public Internet when not in use.
- Regularly audit public-facing assets to identify and remove unnecessary exposure.
- Implement proper security headers even on non-production systems.
