---
certifications: []
description: ''
kind: trust-center
layout: security
name: Patientfi Trust Center
name_suffix: Trust Center
overview: PatientFi maintains a public trust center covering its security and compliance posture.
provider_name: PatientFi
provider_slug: patientfi
slug: patientfi-trust-center
source_filename: patientfi-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.patientfi.com/\npresent: true\nreadable: false\nplatform: Thoropass (formerly Laika)\nplatform_evidence: https://laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js\ncertifications: []\nnote: >-\n  PatientFi operates a real, dedicated Trust Center at trust.patientfi.com — a provider-controlled\n  subdomain that returns HTTP 200 with <title>Trust Center</title> and loads the Thoropass/Laika\n  trust-center bundle. It is NOT a soft 404 and NOT a parked host; it is a deliberately deployed\n  compliance surface. But the served HTML is 814 bytes of shell: every certification, document and\n  subprocessor is fetched client-side from the Thoropass API after script execution, so a crawler,\n  an agent, or a procurement team's automated vendor review receives ZERO machine-readable\n  compliance signal. No SOC 2, ISO 27001, PCI DSS, HIPAA or FedRAMP string appears anywhere in the\n  response body. Certifications\
  \ are therefore recorded as an empty list with readable:false, NOT as\n  absent — the distinction matters, and this is the provider's to fix.\n  Consequently no `type: Compliance` pointer is emitted in apis.yml; the `type: TrustCenter`\n  pointer is emitted because the surface demonstrably exists.\nprobes:\n- url: https://trust.patientfi.com/\n  status: 200\n  content_type: text/html\n  bytes: 814\n  title: Trust Center\n- url: https://patientfi.com/security/\n  status: 404\n- url: https://patientfi.com/.well-known/security.txt\n  status: 403\n  note: nginx edge blocks the entire /.well-known/ prefix — see well-known/patientfi-well-known.yml\nremedy: >-\n  Server-render the certification list, or publish a machine-readable summary (a JSON document\n  or a /.well-known/ pointer) alongside the SPA, so an automated vendor review can read the\n  posture without executing scripts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patientfi/refs/heads/main/security/patientfi-trust-center.yml
summary_line: trust center published
tags:
- healthcare-financing
- patient-financing
- consumer-lending
- Point of Sale Financing
- buy-now-pay-later
- Fintech
- Payments
- embedded-finance
- aesthetics
- plastic-surgery
- medspa
- cosmetic-dental
- fertility
- audiology
- practice-management
trust_url: ''
---
