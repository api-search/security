---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dice.fm
  spf: true
hosts:
- cert_expires: Sep 21 19:15:51 2026 GMT
  host: dice.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DICE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DICE
provider_slug: dice
slug: dice-domain-security
source_filename: dice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dice.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dice.fm\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dice/refs/heads/main/security/dice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Live Events
- Ticketing
- Music
- Events
- Entertainment
- Mobile
- Marketplace
- Discovery
---
