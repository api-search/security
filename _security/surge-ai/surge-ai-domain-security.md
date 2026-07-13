---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: surgehq.ai
  spf: true
hosts:
- cert_expires: Sep  7 02:33:50 2026 GMT
  host: www.surgehq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 12:55:46 2026 GMT
  host: app.surgehq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Surge Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surge AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Surge AI
provider_slug: surge-ai
slug: surge-ai-domain-security
source_filename: surge-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.surgehq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:33:50 2026 GMT\n  hsts: false\n- host: app.surgehq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:55:46 2026 GMT\n  hsts: false\ndomains:\n- domain: surgehq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surge-ai/refs/heads/main/security/surge-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Human Data
- RLHF
- SFT
- Rubrics
- Verifiers
- RL Environments
- Multimodal
- Internationalization
- Labeling
---
