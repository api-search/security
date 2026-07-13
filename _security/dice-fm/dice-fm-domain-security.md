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
- cert_expires: Sep 21 19:15:51 2026 GMT
  host: mio.dice.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: partners-endpoint.dice.fm
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dice Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DICE, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DICE
provider_slug: dice-fm
slug: dice-fm-domain-security
source_filename: dice-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dice.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mio.dice.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partners-endpoint.dice.fm\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dice.fm\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dice-fm/refs/heads/main/security/dice-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Ticketing
- Live Music
- Events
- Tickets
- GraphQL
- Entertainment
- Partner API
---
