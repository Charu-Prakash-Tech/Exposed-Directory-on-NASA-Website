# Exposed Directory on NASA Website

## Issue Overview
While browsing the web, I discovered an exposed directory on NASA's official website, allowing public access to files and folders. This poses a potential risk of unauthorized access to sensitive information, impacting the integrity of NASA's systems.

## Affected URL
[https://spdf.gsfc.nasa.gov/pub/](https://spdf.gsfc.nasa.gov/pub/)

## Discovery Method
The directory was discovered unintentionally using a basic search engine query:

The query revealed a directory listing that should not be publicly accessible.

## Impact
This vulnerability falls under the **Information Disclosure** category. The exposed directory allows:
- Unauthorized access to files and folders.
- Enumeration of the directory structure for reconnaissance.
- Analysis of file contents or metadata, which may provide sensitive insights.
- Increased risk of exploitation by attackers.

Such **Information Disclosure** vulnerabilities are often a result of **Security Misconfiguration** (OWASP A5:2021), highlighting a failure to disable directory indexing or properly restrict access to sensitive files.

## Steps to Reproduce
1. Use the search query: `intitle:index of`
2. Navigate to the affected URL: [https://spdf.gsfc.nasa.gov/pub/](https://spdf.gsfc.nasa.gov/pub/)
3. Observe the directory contents displayed instead of a default web page.

## Recommended Actions
To mitigate the issue, the following steps are recommended:
- **Disable directory indexing** for the affected directory.
- **Review and secure other public directories** to ensure they are not exposed unnecessarily.
- **Implement access controls** to restrict public access where required.

## OWASP Criteria
This vulnerability is classified as:
- **Information Disclosure**: Unintentionally exposed data that could be exploited.
- **A5:2021 - Security Misconfiguration**: Allowing public directory indexing without proper access control.

## Good-Faith Disclosure
This report is submitted with the intent to assist NASA in improving its cybersecurity posture. If additional details or clarification are needed, please feel free to reach out.

---

### Author
**M.K. Charu Prakash**  
Passionate cybersecurity enthusiast and penetration tester, committed to making the digital world more secure.
