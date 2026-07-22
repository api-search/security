---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w4games.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: w4.gd
  spf: false
hosts:
- cert_expires: Sep 15 06:58:43 2026 GMT
  host: www.w4games.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:02:40 2026 GMT
  host: docs.w4.gd
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: W4 Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for W4 Games, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: W4 Games
provider_slug: w4-games
slug: w4-games-domain-security
source_filename: w4-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.w4games.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:58:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.w4.gd\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:02:40 2026 GMT\n  hsts: false\ndomains:\n- domain: w4games.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: w4.gd\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/w4-games/refs/heads/main/security/w4-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Gaming
- Game Development
- Godot
- Multiplayer
- Backend as a Service
- SDK
- Cloud
- Game Servers
- Realtime
---
