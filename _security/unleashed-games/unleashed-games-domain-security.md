---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unleashedgames.com
  spf: false
hosts:
- cert_expires: Aug 25 20:29:50 2026 GMT
  host: www.unleashedgames.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Unleashed Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unleashed Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Unleashed Games
provider_slug: unleashed-games
slug: unleashed-games-domain-security
source_filename: unleashed-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unleashedgames.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 20:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: unleashedgames.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unleashed-games/refs/heads/main/security/unleashed-games-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Gaming
- Video Games
- RPG
- Co-Op Games
- Cross-Platform
- Social Gaming
---
