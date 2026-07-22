---
certifications:
- verified
- status
- detail
- frameworks_probed
- probe_result
- note
description: ''
kind: trust-center
layout: security
name: Linte Trust Center
name_suffix: Trust Center
overview: Linte maintains a public trust center documenting verified, status, detail, frameworks_probed, probe_result, and note compliance.
provider_name: Linte
provider_slug: linte
slug: linte-trust-center
source_filename: linte-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://trust.linte.com\ntrust_center:\n  present: true\n  url: https://trust.linte.com\n  title: Linte Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    Page serves the Vanta trust-center application (data-signature-manifest-url\n    https://assets.vanta.com/static/signature-manifest.*.json), slug id\n    347btb95roz4tszsekwuc6. Content is distinct from the linte.com wildcard\n    application shell, confirming a real, separately hosted property.\ncertifications:\n  verified: []\n  status: not_verified\n  detail: >-\n    The Vanta trust center renders its certification list client-side and the\n    underlying Vanta API requires authorization (api.vanta.com returned 401\n    Unauthorized), so no certification name could be read from the public HTML.\n    NO certifications are asserted here. Operating a Vanta trust center commonly\n    accompanies a SOC 2 program, but that is an inference, not evidence, and is\n \
  \   deliberately not recorded as a finding.\n  frameworks_probed:\n  - SOC 2\n  - ISO 27001\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - GDPR\n  - LGPD\n  probe_result: none readable from public HTML\n  note: >-\n    linte.com/soc2-iso27001-o-que-sao-por-que-sao-importantes is an educational\n    blog article explaining what SOC 2 and ISO 27001 are. It is NOT a claim by\n    Linte to hold either certification and was not treated as one.\nsubprocessors:\n  published: unknown\n  url: null\ndocuments:\n  gated: unknown\n  note: Vanta trust centers typically gate audit reports behind an NDA request flow.\nrelated:\n  security_overview: https://www.linte.com/seguranca\n  responsible_disclosure: https://www.linte.com/seguranca#divulgacao-responsavel\n  privacy_policy: https://www.linte.com/politica-de-privacidade\n  terms_of_use: https://www.linte.com/termos-de-uso\nfollow_up: >-\n  Re-run against trust.linte.com with a headless browser (or an authorized Vanta\n  API token) to read the rendered\
  \ certification list, then upgrade\n  certifications.verified[] and, only if named certs are confirmed, add a\n  `Compliance` pointer to apis.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linte/refs/heads/main/security/linte-trust-center.yml
summary_line: verified, status, detail, frameworks_probed, probe_result, note
tags:
- Company
- Contract Lifecycle Management
- Legal Tech
- Document Automation
- Artificial Intelligence
- Contract Management
- Legal Operations
- Electronic Signature
- Business Intelligence
- Brazil
- SaaS
trust_url: ''
---
