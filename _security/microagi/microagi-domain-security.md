---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: microagi.ai
  spf: false
hosts:
- cert_expires: Aug 28 18:27:00 2026 GMT
  host: www.microagi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microagi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microagi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Microagi
provider_slug: microagi
slug: microagi-domain-security
source_filename: microagi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microagi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: microagi.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microagi/refs/heads/main/security/microagi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- AGI
- Embodied AI
- Physical AI
- Research Lab
- Deep Tech
---
