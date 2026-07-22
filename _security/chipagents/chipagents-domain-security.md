---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chipagents.ai
  spf: true
hosts:
- cert_expires: Sep  2 00:10:25 2026 GMT
  host: chipagents.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chipagents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChipAgents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChipAgents
provider_slug: chipagents
slug: chipagents-domain-security
source_filename: chipagents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chipagents.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:10:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chipagents.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chipagents/refs/heads/main/security/chipagents-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Semiconductors
- Chip Design
- EDA
- Verification
- Agentic AI
- Developer Tools
---
