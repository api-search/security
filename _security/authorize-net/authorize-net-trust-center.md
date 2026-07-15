---
certifications:
- PCI DSS
- SSAE-18 (SOC 1)
- Sarbanes-Oxley (SOX)
description: Authorize.Net's security & compliance posture, captured from the Data Security Compliance knowledge-base article. Authorize.Net is a Visa Solutions / Visa Acceptance (formerly CyberSource / a Visa company) payment gateway and validates its compliance annually via external auditors. Certifications are provided to merchants on request through a Support Case rather than a public trust portal, which is why the automated trust-center probe (which requires a trust.<domain> page) recorded nothing — this is the searched, human-verified fill.
kind: trust-center
layout: security
name: Authorize Net Trust Center
name_suffix: Trust Center
overview: Authorize.net maintains a public trust center documenting PCI DSS, SSAE-18 (SOC 1), and Sarbanes-Oxley (SOX) compliance.
provider_name: Authorize.net
provider_slug: authorize-net
slug: authorize-net-trust-center
source_filename: authorize-net-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://support.authorize.net/knowledgebase/article/000002490/\nurl: https://support.authorize.net/knowledgebase/article/000002490/\ndescription: >-\n  Authorize.Net's security & compliance posture, captured from the Data Security\n  Compliance knowledge-base article. Authorize.Net is a Visa Solutions / Visa\n  Acceptance (formerly CyberSource / a Visa company) payment gateway and validates\n  its compliance annually via external auditors. Certifications are provided to\n  merchants on request through a Support Case rather than a public trust portal,\n  which is why the automated trust-center probe (which requires a trust.<domain>\n  page) recorded nothing — this is the searched, human-verified fill.\ncertifications:\n  - {name: PCI DSS, note: Renewed annually via external security scans; Authorize.Net operates as a PCI-compliant payment gateway / service provider. Level not stated on the public page.}\n  - {name:\
  \ SSAE-18 (SOC 1), availability: on request via Support Case, cadence: annual, note: Statement on Standards for Attestation Engagements No. 18 report on internal controls; also referred to as SOC 1.}\n  - {name: Sarbanes-Oxley (SOX), cadence: annual, note: Annual validation by external auditors for applicable SOX provisions.}\ncompliance_alignment:\n  - {name: HIPAA, note: Compliance validated against applicable federal/state privacy law.}\n  - {name: GLBA, note: Gramm-Leach-Bliley Act.}\n  - {name: California SB 1386, note: State breach-notification law.}\nreport_access:\n  soc_reports: SSAE-18 / SOC 1 report provided to merchants on request by submitting a Support Case.\n  pci_verification: PCI compliance verifiable via the Visa Global Registry of Service Providers.\n  partner: Partnered with SecurityMetrics to help merchants validate their own PCI DSS compliance.\ndocs:\n  - https://support.authorize.net/knowledgebase/article/000002490/\n  - https://support.authorize.net/knowledgebase/Knowledgearticle/?code=KA-04449\n\
  evidence:\n  - {source: https://support.authorize.net/knowledgebase/article/000002490/, keywords: [pci dss, ssae-18, soc 1, sarbanes-oxley, hipaa, glba]}\n  - {source: 'https://support.authorize.net/knowledgebase/Knowledgearticle/?code=KA-04449', keywords: [visa global registry of service providers, pci compliance]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authorize-net/refs/heads/main/security/authorize-net-trust-center.yml
summary_line: PCI DSS, SSAE-18 (SOC 1), Sarbanes-Oxley (SOX)
tags:
- Accept.js
- Credit Cards
- eChecks
- Fraud Detection
- Payment Gateway
- Payments
- Recurring Billing
- Transactions
trust_url: https://support.authorize.net/knowledgebase/article/000002490/
---
