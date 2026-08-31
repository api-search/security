---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hutchgames.com
  spf: true
hosts:
- cert_expires: Sep  1 20:24:08 2026 GMT
  host: hutchgames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hutch Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hutch Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hutch Games
provider_slug: hutch-games
slug: hutch-games-domain-security
source_filename: hutch-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hutchgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:24:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hutchgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hutch-games/refs/heads/main/security/hutch-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Entertainment
- Gaming
- Mobile Games
- Game Development
- Racing Games
- Free To Play
---
