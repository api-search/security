---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: methodical.com
  spf: true
hosts:
- cert_expires: Oct  4 22:05:24 2026 GMT
  host: www.methodical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Methodical Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Methodical Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Methodical Games
provider_slug: methodical-games
slug: methodical-games-domain-security
source_filename: methodical-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.methodical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: methodical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/methodical-games/refs/heads/main/security/methodical-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Games
- Game Development
- Multiplayer
- Game Studio
- Entertainment
- Interactive Media
---
