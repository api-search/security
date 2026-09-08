---
api_specs:
- filename: plumma-connect-openapi.yml
  format: yaml
  label: Plumma CONNECT API
  slug: plumma-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/openapi/plumma-connect-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Plumma Trust Center
name_suffix: Trust Center
overview: Plumma maintains a public trust center covering its security and compliance posture.
provider_name: Plumma
provider_slug: plumma
slug: plumma-trust-center
source_filename: plumma-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nprobe: true\npublished: false\nurl: null\nsource: >-\n  0-working/probe-security-programs.py (trust./security. subdomains and /trust, /security,\n  /compliance paths — no hit) plus a full read of the provider's own Security & Compliance\n  document, retrieved from the documentation content API at\n  https://connect.plumma.it/plumma-connect-docs/#security\ncertifications: []\nnote: >-\n  NO TRUST CENTER EXISTS, AND NO CERTIFICATION IS HELD. There is no trust.plumma.it, no\n  security.plumma.it, and no /trust or /compliance path on any Plumma host. What Plumma does\n  publish is a single dated document — \"Security & Compliance\", V1.1, 21/12/2025 — inside the\n  documentation portal. It is a real and reasonably detailed posture statement, and it is\n  explicit that the standards it names are aspirational: its own heading is \"Suggested\n  Reference Standards\" and the text reads \"While we may not yet hold formal certifications,\n \
  \ we are committed to adhering to the best practices defined by the following security and\n  quality standards\", listing ISO 27001 and SOC 2 Type I/II. Anyone reading this profile\n  must not credit Plumma with either. The GDPR claim is different in kind — it rests on the\n  stated architecture (a pass-through gateway that persists no personal data at rest) rather\n  than on an audit. No third-party attestation, audit report or certificate registry entry\n  is available to check any of it against. `TrustCenter` is NOT emitted; `Compliance` is,\n  pointing at the published document, because a formal compliance posture document does\n  exist even though no certification does.\nposture_summary: conformance/plumma-conformance.yml#compliance\nevidence:\n- {source: 'https://connect.plumma.it/plumma-connect-docs/#security', status: 200, document: 'Security & Compliance V1.1, 21/12/2025'}\n- {source: 'trust.plumma.it', status: no-such-host}\n- {source: 'security.plumma.it', status: no-such-host}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/security/plumma-trust-center.yml
summary_line: trust center published
tags:
- Telecommunications
- Network APIs
- Italy
- Europe
- GSMA Open Gateway
- CAMARA
- API Aggregator
- Fraud Prevention
- Identity Verification
- SIM Swap
- KYC
- Age Verification
- Number Verification
- Telco Intelligence
- Software Development
trust_url: ''
---
