---
certifications:
- HITRUST r2
- SOC 2 Type II
- EHNAC
- DirectTrust
- WebTrust for Certification Authorities
- HIPAA
description: ''
kind: trust-center
layout: security
name: Surescripts Trust Center
name_suffix: Trust Center
overview: Surescripts maintains a public trust center documenting HITRUST r2, SOC 2 Type II, EHNAC, DirectTrust, WebTrust for Certification Authorities, and HIPAA compliance.
provider_name: Surescripts
provider_slug: surescripts
slug: surescripts-trust-center
source_filename: surescripts-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nprobe: true\nsource: https://surescripts.com/why-surescripts/certifications-and-accreditations\nurl: https://surescripts.com/why-surescripts/certifications-and-accreditations\nnote: >-\n  probe-security-programs.py found no trust.surescripts.com / security.surescripts.com host\n  (both NXDOMAIN, 2026-08-15) and no /trust, /security or /compliance path. Surescripts does\n  publish a named certifications and accreditations page on its own site, which carries the\n  certification detail a trust center would, so this artifact is recorded as searched from that\n  page rather than from a hosted trust portal.\ncertifications:\n  - HITRUST r2\n  - SOC 2 Type II\n  - EHNAC\n  - DirectTrust\n  - WebTrust for Certification Authorities\n  - HIPAA\nprograms:\n  - name: HITRUST r2 (Risk-Based, 2-Year) Certified\n    detail: >-\n      Demonstrates that key platforms within Surescripts solutions and their supporting\n      infrastructure meet HITRUST's\
  \ highest level of information security and compliance;\n      more than 300 requirements were met.\n  - name: SOC 2 Type II\n    detail: >-\n      Annual Service Organization Controls 2 Type II report issued by an independent AICPA\n      audit firm, assessing design and operating effectiveness of controls against the\n      security, availability and confidentiality trust principles.\n  - name: EHNAC\n    detail: >-\n      Participation in the Electronic Healthcare Network Accreditation Commission programme,\n      a federally recognised standards development organisation and non-profit accrediting\n      body for transactional quality, operational efficiency and healthcare data security.\n  - name: DirectTrust\n    detail: >-\n      Accredited for Health Information Service Provider (HISP), Registration Authority (RA),\n      Certificate Authority (CA) and Privacy & Security operations in support of DirectTrust\n      messaging for Clinical Direct Messaging.\n  - name: Surescripts Certification\
  \ Practice Statement (CPS)\n    detail: >-\n      Publicly available document describing Surescripts' certificate practices and policies,\n      required by WebTrust for Certification Authorities. Surescripts operates as a Certificate\n      Authority and Registration Authority and issues the digital certificates used for\n      DirectTrust products and the mutually authenticated TLS connections customers use to\n      reach its APIs.\nevidence:\n  - source: https://surescripts.com/why-surescripts/certifications-and-accreditations\n    status: 200\n    keywords:\n      - HITRUST\n      - SOC 2 Type II\n      - EHNAC\n      - DirectTrust\n      - Certification Practice Statement\n  - source: https://care-coordination.surescripts.net\n    kind: tls-chain\n    detail: >-\n      Live TLS probe 2026-08-15 confirms the CPS in practice - the API host's certificate is\n      issued by \"Surescripts Issuing Certification Authority\" under \"Surescripts Root\n      Certification Authority\".\nnegative_findings:\n\
  \  - host: trust.surescripts.com\n    result: NXDOMAIN\n  - host: security.surescripts.com\n    result: NXDOMAIN\n  - path: /.well-known/security.txt\n    result: 404 on surescripts.com, www.surescripts.com and docs.surescripts.com\n  - item: vulnerability disclosure / bug bounty programme\n    result: >-\n      None found. No security.txt Policy or Contact, no HackerOne/Bugcrowd/Intigriti listing,\n      no responsible-disclosure page. No VulnerabilityDisclosure or Security pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surescripts/refs/heads/main/security/surescripts-trust-center.yml
summary_line: HITRUST r2, SOC 2 Type II, EHNAC, DirectTrust, WebTrust for Certification Authorities, HIPAA
tags:
- Healthcare
- e-Prescribing
- Health Information Network
- NCPDP SCRIPT
- Medication History
- Prior Authorization
- Interoperability
- FHIR
- Formulary
- Eligibility
- Real-Time Prescription Benefit
- Mutual TLS
- Gated
trust_url: https://surescripts.com/why-surescripts/certifications-and-accreditations
---
