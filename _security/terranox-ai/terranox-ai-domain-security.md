---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: terranox.ai
  spf: true
hosts:
- cert_expires: Oct  9 02:48:45 2026 GMT
  host: terranox.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terranox Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terranox AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Terranox AI
provider_slug: terranox-ai
slug: terranox-ai-domain-security
source_filename: terranox-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terranox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terranox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terranox-ai/refs/heads/main/security/terranox-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Energy
- Nuclear
- Uranium
- Mineral Exploration
- Geoscience
- Climate Tech
- Y Combinator
---
