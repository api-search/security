---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jagex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: runescape.com
  spf: true
hosts:
- cert_expires: Sep 27 09:57:43 2026 GMT
  host: www.jagex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 11:47:35 2026 GMT
  host: secure.runescape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: services.runescape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jagex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jagex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jagex
provider_slug: jagex
slug: jagex-domain-security
source_filename: jagex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jagex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:57:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.runescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.runescape.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jagex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: runescape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jagex/refs/heads/main/security/jagex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Games
- RuneScape
- MMORPG
- Video Games
- Game Data
- Grand Exchange
- Hiscores
- Player Data
---
