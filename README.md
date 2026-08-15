# OWASP Juice Shop Penetration Test

## Overview

Black-box web application security assessment of a locally hosted OWASP Juice Shop instance. The assessment was performed manually using Burp Suite Professional, browser developer tools, reconnaissance, endpoint mapping, authenticated and unauthenticated testing, manual exploitation, proof-of-concept verification, CVSS v3.1 scoring, and remediation analysis.

## Assessment Summary

- **Target:** OWASP Juice Shop — local instance (`http://127.0.0.1:3000`)
- **Assessment Type:** Black-box web application penetration test
- **Tools:** Burp Suite Professional, Chromium/Firefox Developer Tools
- **Findings:** 6 confirmed vulnerabilities
- **Severity Breakdown:** 1 Critical, 2 High, 2 Medium, 1 Low
- **Assessment Date:** 12 August 2026

## Confirmed Vulnerabilities

| # | Finding | Severity | CVSS v3.1 |
|---|---|---|---:|
| 1 | SQL Injection Leading to Authentication Bypass (Admin Account Takeover) | Critical | 9.8 |
| 2 | Broken Access Control (IDOR) — Unauthorized Access to Other Users' Shopping Baskets | High | 8.1 |
| 3 | Reflected Cross-Site Scripting (XSS) in Product Search | Medium | 6.1 |
| 4 | Sensitive/Confidential Information Disclosure via Exposed FTP Directory | High | 7.5 |
| 5 | Verbose Error Messages / Stack Trace Disclosure | Medium | 5.3 |
| 6 | Exposed Application Metrics Endpoint (Information Disclosure) | Low | 5.3 |

## Report

The complete 20-page penetration test report contains methodology, affected endpoints, reproduction steps, proof-of-concept evidence, impact analysis, CVSS scoring, and remediation recommendations.

**Report file:** `reports/Juice_Shop_Penetration_Test_Report.pdf`

## Professional Note

Testing was performed against a local OWASP Juice Shop training environment for educational and authorized security assessment purposes. No real-world production system was targeted.

## Disclaimer

This repository is provided for educational and authorized security-testing purposes only. Do not use the documented techniques against systems without explicit permission.
