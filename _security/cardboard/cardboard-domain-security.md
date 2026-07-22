---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usecardboard.com
  spf: true
hosts:
- cert_expires: Oct  7 03:10:45 2026 GMT
  host: usecardboard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cardboard
provider_slug: cardboard
slug: cardboard-domain-security
source_filename: cardboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usecardboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:10:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usecardboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardboard/refs/heads/main/security/cardboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Editing
- Artificial Intelligence
- Video
- Creative Tools
- Media
- SaaS
- Browser-Based
- Y Combinator
---
