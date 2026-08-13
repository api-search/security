---
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Fevo Trust Center
name_suffix: Trust Center
overview: Fevo maintains a public trust center documenting SOC 2 compliance.
provider_name: Fevo
provider_slug: fevo
slug: fevo-trust-center
source_filename: fevo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://www.fevo.com/security\nname: FEVO Security\nurl: https://www.fevo.com/security\nplatform: self-hosted page (Webflow marketing site); no third-party trust portal\nnote: >-\n  FEVO publishes a single, reasonably detailed security page covering organizational,\n  cloud, access and vendor-risk controls. Read it precisely: FEVO says its Information\n  Security Program \"follows the criteria set forth by the SOC 2 Framework\" and that it\n  \"undergoes independent third-party assessments\". It does NOT claim a completed SOC 2\n  Type I or Type II report, does not name an auditor, does not offer a report under NDA,\n  and names no other certification. No ISO 27001, PCI DSS, HIPAA, FedRAMP, GDPR or CCPA\n  certification is asserted on this page (a CCPA Notice exists separately in the site\n  footer). No downloadable evidence, no subprocessor list, no SIG/CAIQ.\n\ncertifications:\n  - name: SOC 2\n    status: framework-alignment-claimed\n\
  \    type: null\n    auditor: null\n    report_available: false\n    evidence: >-\n      \"Our Information Security Program follows the criteria set forth by the SOC 2\n      Framework.\" No report, date, scope or auditor is published.\n\ncontrols_published:\n  organizational:\n    - Information Security Program communicated org-wide\n    - Independent third-party assessments of security and compliance controls\n    - Independent third-party penetration test at least annually\n    - Documented roles and responsibilities; policies reviewed and accepted by staff\n    - Security awareness training (phishing, password management)\n    - Confidentiality agreements signed before first day\n    - Background checks on all new team members\n  cloud:\n    - Services hosted on AWS\n    - Data hosted on AWS and GCP databases, all located in the United States\n    - All databases encrypted at rest\n    - Applications encrypted in transit with TLS/SSL\n    - Vulnerability scanning and active threat\
  \ monitoring\n    - Logging and monitoring of cloud services\n    - Backups via the hosting provider; monitoring alerts on failures\n    - Documented incident response with escalation, rapid mitigation and communication\n  access:\n    - Access to cloud infrastructure limited to authorized employees by role\n    - SSO, 2FA and strong password policies where available\n    - Least-privilege identity and access management\n    - Quarterly access reviews for sensitive systems\n    - Minimum password complexity requirements; company-issued password manager\n  vendor_risk:\n    - At least annual risk assessments, including fraud considerations\n    - Vendor review before authorizing a new vendor\n\ndata_residency: United States (AWS and GCP)\ndata_retention: 'transactional data retained up to six years (source: Order API FAQ)'\n\npayment_security_note: >-\n  Not claimed on the security page, but observed directly: a live FEVO offer page loads the\n  Braintree web SDK 3.99.0 (hosted fields,\
  \ 3-D Secure, data collector) and Shift4, meaning\n  card data is captured in vendor-hosted fields rather than by FEVO. FEVO makes no PCI DSS\n  statement of its own.\n\ncontact: security_questions@fevo.com\n\ngaps:\n  - No completed SOC 2 report offered, even under NDA\n  - No auditor, report date or scope named\n  - No subprocessor list\n  - No status/incident history page\n  - No RFC 9116 /.well-known/security.txt on any FEVO host\n  - No bug bounty or coordinated disclosure policy\n  - Page footer still reads \"© 2023 FEVO Inc.\"\n\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://www.fevo.com/security\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fevo/refs/heads/main/security/fevo-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Ticketing
- Events
- Group Sales
- Social Commerce
- E-Commerce
- Checkout
- Sports
- Live Entertainment
- Embedded Commerce
trust_url: https://www.fevo.com/security
---
