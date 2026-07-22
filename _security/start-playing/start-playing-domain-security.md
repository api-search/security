---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: startplaying.games
  spf: true
hosts:
- cert_expires: Oct  1 04:56:10 2026 GMT
  host: startplaying.games
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Start Playing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Start Playing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Start Playing
provider_slug: start-playing
slug: start-playing-domain-security
source_filename: start-playing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: startplaying.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:56:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: startplaying.games\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/start-playing/refs/heads/main/security/start-playing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Gaming
- Tabletop RPG
- Marketplace
- Entertainment
- Community
- Booking
- Consumer
---
