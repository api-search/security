---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caretta.so
  spf: true
hosts:
- cert_expires: Oct  2 17:23:14 2026 GMT
  host: www.caretta.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caretta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caretta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caretta
provider_slug: caretta
slug: caretta-domain-security
source_filename: caretta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caretta.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:23:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: caretta.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caretta/refs/heads/main/security/caretta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Real-Time
- Conversation Intelligence
- Revenue Operations
- Y Combinator
---
