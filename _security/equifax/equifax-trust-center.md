---
certification_count: 3
certifications:
- FedRAMP
- NIST Cybersecurity Framework (CSF)
- third-party certifications and authorizations (aggregate)
description: Equifax operates a SafeBase trust center at trust.equifax.com and publishes an annual Security Annual Report plus a public security controls framework on GitHub. A separate portal, securityreports.equifax.com, distributes security reports but is login-walled to approved Equifax business users.
kind: trust-center
layout: security
name: Equifax Trust Center
name_suffix: Trust Center
overview: Equifax maintains a public trust center documenting FedRAMP, NIST Cybersecurity Framework (CSF), and third-party certifications and authorizations (aggregate) compliance.
provider_name: Equifax
provider_slug: equifax
slug: equifax-trust-center
source_filename: equifax-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nsource: https://www.equifax.com/about-equifax/security/\nurl: https://trust.equifax.com/\nplatform: SafeBase\nplatform_evidence: >-\n  trust.equifax.com is a CNAME to equifax.portals.safebase.io (dig, 2026-09-06) — a\n  SafeBase-hosted trust center.\nreadable_by_crawler: false\nreadable_note: >-\n  Both https://trust.equifax.com/ and the underlying https://equifax.portals.safebase.io/\n  answered HTTP 403 with a Cloudflare \"Just a moment...\" interstitial to every request\n  this pipeline made, including with a browser User-Agent. The portal demonstrably exists;\n  we did not evade the challenge, so the certification list BEHIND it is not recorded here.\n  Only certifications Equifax states on pages we could actually read are listed below.\ndescription: >-\n  Equifax operates a SafeBase trust center at trust.equifax.com and publishes an annual\n  Security Annual Report plus a public security controls framework on GitHub.\
  \ A separate\n  portal, securityreports.equifax.com, distributes security reports but is login-walled to\n  approved Equifax business users.\ncertifications:\n  - name: FedRAMP\n    status: Ready for Agency Authorization\n    evidence: https://www.equifax.com/about-equifax/security/\n    quote: '\"FedRAMP Ready for Agency Authorization\"'\n  - name: NIST Cybersecurity Framework (CSF)\n    status: assessed\n    score: '4.4 (2025)'\n    evidence: https://www.equifax.com/about-equifax/security/\n    quote: >-\n      \"a 2025 National Institute of Standards Technology (NIST) Cybersecurity Framework\n      (CSF) score of 4.4 - an increase from last year's score of 4.3\"\n  - name: third-party certifications and authorizations (aggregate)\n    count: 52\n    status: claimed\n    evidence: https://www.equifax.com/about-equifax/security/\n    quote: >-\n      \"52 Certifications and authorizations obtained from outside auditors, validating our\n      depth and rigor\"\n    note: >-\n      Equifax\
  \ states the COUNT but does not enumerate the 52 on this page. The individual\n      certificates are presumably behind the trust center and securityreports portal. Not\n      itemised here because we could not read them.\npublic_artifacts:\n  - name: Equifax Security Annual Report\n    url: https://www.equifax.com/about-equifax/security/annual-report/\n    status: 200\n    access: public\n  - name: Equifax Security Controls Framework\n    url: https://github.com/Equifax-Public/SecurityControlsFramework\n    access: public\n    note: >-\n      Equifax states \"thousands of users across 70 countries leverage our public security\n      controls framework\"; the repository is the only one in the Equifax-Public GitHub org.\n  - name: Equifax Security Reports portal\n    url: https://securityreports.equifax.com/\n    status: 200\n    access: gated\n    gate: >-\n      \"access to Equifax Security Reports is for Equifax Business users only. Access must\n      be approved internally prior to\
  \ being granted.\"\nevidence:\n  - source: https://www.equifax.com/about-equifax/security/\n    status: 200\n    keywords: [fedramp ready, nist csf 4.4, 52 certifications, report a vulnerability]\n  - source: https://trust.equifax.com/\n    status: 403\n    kind: Cloudflare bot challenge — page exists, body not readable by this crawler\n  - source: https://securityreports.equifax.com/\n    status: 200\n    kind: login wall\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equifax/refs/heads/main/security/equifax-trust-center.yml
summary_line: FedRAMP, NIST Cybersecurity Framework (CSF), third-party certifications and authorizations (aggregate)
tags:
- Credit
- Credit History
- Credit Reporting
- Identity
- Fraud Detection
- Fortune 1000
trust_url: https://trust.equifax.com/
---
