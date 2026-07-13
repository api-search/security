---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: scale.com
  spf: true
hosts:
- cert_expires: Sep 23 15:40:03 2026 GMT
  host: scale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 19:18:59 2026 GMT
  host: api-reference.scale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:14:12 2026 GMT
  host: api.scale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scale Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scale AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Scale AI
provider_slug: scale-ai
slug: scale-ai-domain-security
source_filename: scale-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:40:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-reference.scale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:18:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.scale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:14:12 2026 GMT\n  hsts: null\ndomains:\n- domain: scale.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-ai/refs/heads/main/security/scale-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Engine
- Labeling
- RLHF
- GenAI Platform
- Donovan
- Defense AI
- LiDAR
- Sensor Fusion
- REST API
---
