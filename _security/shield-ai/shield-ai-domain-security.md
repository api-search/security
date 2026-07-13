---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shield.ai
  spf: true
hosts:
- cert_expires: Oct  4 22:23:40 2026 GMT
  host: shield.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shield Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shield AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shield AI
provider_slug: shield-ai
slug: shield-ai-domain-security
source_filename: shield-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shield.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:23:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shield.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shield-ai/refs/heads/main/security/shield-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defense
- Autonomy
- Hivemind
- EdgeOS
- Robotics
- Unmanned Systems
- Mission Software
- Edge AI
- V-BAT
- ITAR
- Swarming
---
