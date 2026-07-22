---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bluestudios.io
  spf: true
hosts:
- cert_expires: Oct 16 01:01:29 2026 GMT
  host: bluestudios.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blue Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blue Studios
provider_slug: blue-studios
slug: blue-studios-domain-security
source_filename: blue-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluestudios.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:01:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluestudios.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-studios/refs/heads/main/security/blue-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Family Tech
- Personal Finance
- FinTech
- EdTech
- Streaming
- Media and Entertainment
- Techstars
---
