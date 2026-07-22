---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 7-chord.com
  spf: true
hosts:
- cert_expires: Dec 13 21:36:52 2026 GMT
  host: 7-chord.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 7 Chord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7 Chord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 7 Chord
provider_slug: 7-chord
slug: 7-chord-domain-security
source_filename: 7-chord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 7-chord.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 21:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 7-chord.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7-chord/refs/heads/main/security/7-chord-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fixed Income
- Bond Pricing
- Artificial Intelligence
- Market Data
- FinTech
- Credit Trading
- Analytics
---
