---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elsewhere.zone
  spf: true
hosts:
- cert_expires: Sep 15 21:11:12 2026 GMT
  host: elsewhere.zone
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elsewhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elsewhere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elsewhere
provider_slug: elsewhere
slug: elsewhere-domain-security
source_filename: elsewhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elsewhere.zone\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:11:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: elsewhere.zone\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsewhere/refs/heads/main/security/elsewhere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Games
- Gaming
- Video Games
- Game Studio
- Generative AI
- Artificial Intelligence
- Consumer
- Entertainment
- San Francisco
- a16z SPEEDRUN
---
