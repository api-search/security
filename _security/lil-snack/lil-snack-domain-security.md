---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lilsnack.com
  spf: true
hosts:
- cert_expires: Sep 14 14:14:51 2026 GMT
  host: www.lilsnack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lil Snack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lil Snack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lil Snack
provider_slug: lil-snack
slug: lil-snack-domain-security
source_filename: lil-snack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lilsnack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lilsnack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lil-snack/refs/heads/main/security/lil-snack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Games
- Gaming
- Daily Games
- Puzzles
- Word Games
- Trivia
- Casual Games
- Media
- Entertainment
- Pop Culture
- Consumer
- Embedded Games
- Advertising
- Sponsorship
---
