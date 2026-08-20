---
certifications:
- SOC 2 Type 2
- PCI DSS
- HIPAA/HITECH Type 1
- CCPA
description: ''
kind: trust-center
layout: security
name: Glia Trust Center
name_suffix: Trust Center
overview: Glia maintains a public trust center documenting SOC 2 Type 2, PCI DSS, HIPAA/HITECH Type 1, and CCPA compliance.
provider_name: Glia
provider_slug: glia
slug: glia-trust-center
source_filename: glia-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://www.glia.com/security\ntype: security-and-compliance-page\ndedicated_trust_center: false\nnote: >-\n  Glia does not run a dedicated trust portal - trust.glia.com does not resolve. Its security and\n  compliance posture is published as a page on the marketing site, which names the attestations\n  it holds directly and the ones it inherits from AWS.\ncertifications:\n- {name: SOC 2 Type 2, held_by: Glia}\n- {name: PCI DSS, held_by: Glia}\n- {name: HIPAA/HITECH Type 1, held_by: Glia}\n- {name: CCPA, held_by: Glia, kind: regulation}\ninherited_from_infrastructure:\n  provider: Amazon Web Services\n  attestations:\n  - ISO/IEC 27001\n  - SSAE-16 SOC 1\n  - SSAE-16 SOC 2\n  - SSAE-16 SOC 3\n  - FedRAMP\n  - FISMA\n  note: >-\n    These are AWS attestations Glia cites as inherited through its hosting, not certifications\n    issued to Glia. Recorded separately so the distinction is not lost.\ncontrols_published:\n\
  - All data encrypted in transit and at rest\n- End-to-end encryption\n- Masking of PII\n- 24/7 intrusion detection\n- Daily manual log review\n- OWASP-based security testing\n- Platform hosted exclusively on AWS\nrelated:\n  vulnerability_disclosure: security/glia-vulnerability-disclosure.yml\n  terms_of_service: https://www.glia.com/security-compliance/terms-of-service\n  privacy_policy: https://www.glia.com/security-compliance/privacy-policy\nevidence:\n- source: https://www.glia.com/security\n  http_status: 200\n  fetched: '2026-08-04'\n  keywords: [soc 2 type 2, pci dss, hipaa, hitech, ccpa, encryption, intrusion detection]\n- source: https://trust.glia.com/\n  http_status: 0\n  fetched: '2026-08-04'\n  note: Does not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glia/refs/heads/main/security/glia-trust-center.yml
summary_line: SOC 2 Type 2, PCI DSS, HIPAA/HITECH Type 1, CCPA
tags:
- Company
- Customer Service
- Contact Center
- Banking
- Credit Unions
- Financial-Services
- Conversational AI
- Voice
- Co-Browsing
- Serverless
trust_url: https://www.glia.com/security
---
