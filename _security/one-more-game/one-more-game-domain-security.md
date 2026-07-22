---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onemoregame.com
  spf: true
hosts:
- cert_expires: Sep 21 23:04:47 2026 GMT
  host: onemoregame.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One More Game Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One More Game, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: One More Game
provider_slug: one-more-game
slug: one-more-game-domain-security
source_filename: one-more-game-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onemoregame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:04:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onemoregame.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-more-game/refs/heads/main/security/one-more-game-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Video Games
- Game Development
- Online Games
- Entertainment
- Studio
---
