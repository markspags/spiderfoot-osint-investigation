# spiderfoot-osint-investigation
OSINT investigation project using SpiderFoot to document suspicious email, domain, IP, and infrastructure risk signals.

# micr0soft-support.com SpiderFoot Investigation

## Overview
This repository documents a simulated OSINT investigation into the suspicious domain **micr0soft-support.com** using SpiderFoot.
The investigation is based on a phishing scenario involving the email:
security-alert@micr0soft-support.com
The goal is to determine whether the domain demonstrates indicators of phishing, typosquatting, or credential harvesting risk.

---

## Scenario
A user reported receiving an email claiming to be from Microsoft, warning of a suspicious login attempt. The email requested the user to reset their password immediately.
The sender address was:
security-alert@micr0soft-support.com
Initial review identified a potential impersonation attempt due to the use of "0" instead of "o" in "Microsoft".

---

## Tools Used
- SpiderFoot (OSINT investigation)

---

## Investigation Workflow
1. Extracted domain from suspicious email
2. Ran SpiderFoot scan using **Investigate mode**
3. Reviewed:
   - Domain Name
   - Whois
   - Similar Domain
   - Affiliate Email Data
4. Assessed indicators for phishing risk

---

## Key Finding
The domain:
micr0soft-support.com
uses **character substitution (0 instead of o)** to imitate Microsoft.
This is a known **typosquatting technique** commonly used in phishing campaigns.

---

## Risk Assessment
Even without confirmed blacklist hits, the domain presents **elevated phishing risk** due to:

- Brand impersonation
- Typosquatting
- Security-themed sender name
- Credential reset lure scenario

---

## Conclusion
The domain is highly suspicious and consistent with phishing activity designed to support **account takeover (ATO)** attacks.
