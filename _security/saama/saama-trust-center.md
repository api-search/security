---
certifications:
- ISO/IEC 27001:2013
- 21 CFR Part 11
- ICH E6 (Good Clinical Practice)
- FIPS 140-2
description: ''
kind: trust-center
layout: security
name: Saama Trust Center
name_suffix: Trust Center
overview: Saama maintains a public trust center documenting ISO/IEC 27001:2013, 21 CFR Part 11, ICH E6 (Good Clinical Practice), and FIPS 140-2 compliance.
provider_name: Saama
provider_slug: saama
slug: saama-trust-center
source_filename: saama-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.saama.com/about/company/security-compliance/\nname: Saama Security & Compliance\nurl: https://www.saama.com/about/company/security-compliance/\nnote: >-\n  Saama does not run a dedicated trust-center host (trust.saama.com and status.saama.com both\n  fail DNS resolution). The \"Trust\" item in the site navigation and https://www.saama.com/security/\n  and https://www.saama.com/about/company/trust/ all resolve to this single Security & Compliance\n  page, which is the company's published trust surface. It names the frameworks its information\n  security management program is aligned to; it does NOT claim third-party certification or\n  attestation for any of them, and no audit report, SOC 2 attestation or certificate download is\n  offered - the only artifact linked is a marketing white paper. Recorded exactly as stated.\naliases:\n- https://www.saama.com/security/\n- https://www.saama.com/about/company/trust/\n\
  certifications:\n- name: ISO/IEC 27001:2013\n  status: aligned\n  evidence: >-\n    \"We maintain an information security management program with defined roles, responsibilities,\n    policies, and procedures. Our program is aligned to: ISO/IEC 27001:2013; 21 CFR Part 11; and\n    ICH E6.\"\n- name: 21 CFR Part 11\n  status: aligned\n  evidence: same \"Our program is aligned to\" statement under Safeguards Practices/Procedures - Organizational\n- name: ICH E6 (Good Clinical Practice)\n  status: aligned\n  evidence: same \"Our program is aligned to\" statement under Safeguards Practices/Procedures - Organizational\n- name: FIPS 140-2\n  status: aligned\n  evidence: >-\n    \"We use industry standard AES 256-bit encryption and cryptographic algorithms, approved in the\n    Federal Information Processing Standard (\"FIPS\" 140-2) security standards publication.\"\nnot_claimed:\n- SOC 2\n- HITRUST\n- FedRAMP\n- PCI DSS\n- HIPAA (named nowhere on the page despite the clinical-data domain)\n\
  - GDPR (named nowhere on the page)\npractices_published:\n- external Chief Information Security Officer appointed\n- separation of admin roles from development and service-delivery teams\n- AWS-hosted SaaS platform and Clinical AI/Analytics-as-a-Service (CaaS)\n- TLS 1.2 and TLS 1.3 in transit; AES-256 at rest\n- SAML, OAuth and LDAP authentication with SSO and Federated Identity Management\n- MFA required for critical systems\n- EDR, CASB, SIEM and WAF deployed\n- DAST, SAST, container vulnerability scanning and black-box manual testing in the SDLC\n- Threat and Vulnerability Management (TVM) program\n- multi-data-center deployment with documented and tested recovery procedures\nai_governance:\n  note: >-\n    The page states a commitment to evolving AI regulation rather than conformance to it.\n  frameworks_referenced:\n  - US Executive Order on Safe, Secure, and Trustworthy Development and Use of Artificial Intelligence (2023)\n  - Canada Artificial Intelligence and Data Act (AIDA)\n\
  \  - EU AI Act\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No coordinated vulnerability disclosure program is published. The page describes INTERNAL\n    Threat and Vulnerability Management (DAST/SAST/scanning) only. There is no security.txt\n    (/.well-known/security.txt returns 404), no security@ contact, no /responsible-disclosure page\n    (that path soft-404s to the homepage), and no HackerOne/Bugcrowd/Intigriti program. No\n    VulnerabilityDisclosure or Security pointer is emitted.\nx-evidence:\n- url: https://www.saama.com/about/company/security-compliance/\n  status: 200\n- url: https://www.saama.com/security/\n  status: 200\n- url: https://www.saama.com/.well-known/security.txt\n  status: 404\n- url: https://www.saama.com/responsible-disclosure/\n  status: 200\n  note: soft-404 - canonical is https://www.saama.com/, not a real page\n- url: https://trust.saama.com/\n  status: <no response>\n  note: DNS NXDOMAIN\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saama/refs/heads/main/security/saama-trust-center.yml
summary_line: ISO/IEC 27001:2013, 21 CFR Part 11, ICH E6 (Good Clinical Practice), FIPS 140-2
tags:
- Life Sciences
- Clinical Trials
- Clinical Data Management
- Analytics
- Artificial Intelligence
- Machine Learning
- Pharmaceuticals
- Healthcare
- Data Platform
- CDISC
trust_url: https://www.saama.com/about/company/security-compliance/
---
