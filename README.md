# Italian-University-Exposure
Passive reconnaissance project focused on mapping and assessing the online attack surface of Italian universities. The analysis identifies critical exposures, outdated systems, and administrative portals accessible from the Internet, providing a real-world overview of systemic vulnerabilities within academic infrastructures.

## Most Relevant Collected Cases

| Case ID | University | Exposure Type | Severity | Link |
|:-------:|:-----------:|:-------------:|:--------:|:----:|
| 01 | UNI-Milano | FTP server on printer (Sharp MX-M502N) | Critical | [View Case](cases/case-01.md) |
| 02 | UNI-Verona | FTP server with anonymous access (ProFTPD) | High | [View Case](cases/case-02.md) |
| 03 | UNI-Padova | OpenStack Dashboard exposed (Padova) | High | [View Case](cases/case-03.md) |
| 04 | UNI-Pisa | OpenStack Dashboard exposed (Pisa) | High | [View Case](cases/case-04.md) |
| 05 | UNI-Bologna | Old Apache/SSL server (Centro ANTARES) | Medium | [View Case](cases/case-05.md) |
| 06 | UNI-Padova | FTP services (no anonymous) exposed | Medium | [View Case](cases/case-06.md) |
| 07 | UNI-Napoli | Multiple "Under Construction" or "Maintenance" portals | Low | [View Case](cases/case-07.md) |
| 08 | UNI-Pisa | SonicWALL web management portals exposed | Low | [View Case](cases/case-08.md) |

## Other Collected Cases

| University | Exposure Type |
|:-----------:|:--------------|
| UNI-Ancona | "Websites under construction" accessible |
| UNI-Napoli Federico II | Offline maintenance pages exposed |
| UNI-Napoli L'Orientale | Web services in construction phase exposed |
| UNI-Campania | Webmin login interface exposed |
| UNI-Pisa | Secondary SonicWALL portal accessible |
| UNI-Cosenza | MyDIMEG login page accessible |
| UNI-Milano | Internal services login page exposed |
| UNI-Genova | U-Gov system login exposed |
| UNI-Milano - Bocconi | Web login page exposed |
| UNI-Milano | ChemBox login exposed |
| UNI-Roma1 | Qlik Sense login page exposed |
| UNI-Firenze | eSlideManager login page exposed |
| UNI-Milano | Giunta fisica login portal exposed |
| UNI-Roma1 | EZproxy login portal exposed |
| UNI-Firenze | SquirrelMail login portal exposed |
| UNI-Salerno | Subversion Edge (SVN) portal exposed |

## Conclusions

This project highlights how many academic institutions maintain publicly accessible services that can introduce unnecessary risks. Even minor or outdated services, when exposed, may serve as entry points for attackers.  
By systematically identifying and categorizing such exposures, this research underscores the importance of proactive surface management and continuous monitoring.  
Future steps could include expanding the scope to additional sectors or automating the detection of these weaknesses for wider security assessments.

## Disclaimer

This project is based exclusively on publicly available information and does not involve any unauthorized access attempts. The objective is to promote awareness about passive exposure risks and encourage better security practices.


