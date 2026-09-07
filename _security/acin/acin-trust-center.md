---
certification_count: 2
certifications:
- ISO/IEC 27001
- Cyber Essentials
description: ''
kind: trust-center
layout: security
name: Acin Trust Center
name_suffix: Trust Center
overview: Acin maintains a public trust center documenting ISO/IEC 27001 and Cyber Essentials compliance.
provider_name: Acin
provider_slug: acin
slug: acin-trust-center
source_filename: acin-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.acin.com/privacy-policy/ (HTTP 200, section \"Security over the internet\") and the\n  Drata-hosted trust center Acin links from its own homepage,\n  https://app.drata.com/trust/118b5648-4aaa-42bf-938c-ca51a6f2be37.\ntrust_center:\n  url: https://app.drata.com/trust/118b5648-4aaa-42bf-938c-ca51a6f2be37\n  platform: Drata\n  linked_from: https://www.acin.com/ (homepage footer)\n  readable: false\n  http_status: 403\n  read_note: >-\n    Both app.drata.com and trust.acin.com return a Cloudflare interstitial (\"Just a moment...\")\n    to a non-browser client, so the certifications, subprocessor list and document requests the\n    trust center itself lists could not be read. The page demonstrably exists — Acin links it from\n    its own homepage — so this is a bot challenge, not a dead pointer. The certifications below are\n    taken from Acin's own privacy policy, not from the trust center.\ncertifications:\n\
  - name: ISO/IEC 27001\n  status: certified\n  claim: >-\n    \"Acin operates an information security management programme that aligns with the ISO 27001\n    standard on information security management and have certified our compliance with this\n    standard.\"\n  evidence: https://www.acin.com/privacy-policy/\n  evidence_status: 200\n  certificate_published: false\n- name: Cyber Essentials\n  status: accredited\n  claim: '\"In addition, Acin has Cyber Essentials accreditation.\"'\n  evidence: https://www.acin.com/privacy-policy/\n  evidence_status: 200\n  certificate_published: false\n  note: UK NCSC scheme; the privacy policy does not state whether this is Cyber Essentials or Cyber Essentials Plus.\nregulatory_context:\n- name: UK GDPR / EU GDPR\n  role: data controller and processor\n  evidence: https://www.acin.com/privacy-policy/\n  note: >-\n    The privacy policy is written to UK/EU GDPR, covers international transfers outside the EEA/UK,\n    and names a breach-notification procedure.\
  \ Acin's customers are tier-one banks, so the platform\n    also sits inside their own operational-resilience regimes (e.g. UK PRA/FCA operational\n    resilience, EU DORA), but Acin publishes no statement of its own about those regimes.\nnot_found:\n- SOC 2 report or attestation\n- PCI DSS\n- HIPAA\n- FedRAMP\n- A public subprocessor list on acin.com\n- A published penetration-test summary\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acin/refs/heads/main/security/acin-trust-center.yml
summary_line: ISO/IEC 27001, Cyber Essentials
tags:
- Company
- Operational Risk
- Risk Management
- Non-Financial Risk
- Financial Services
- Banking
- Compliance
- Regulatory Technology
- Benchmarking
- Data Standards
trust_url: ''
---
