---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agavegames.com
  spf: false
hosts:
- cert_expires: Aug 31 16:03:48 2026 GMT
  host: www.agavegames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agavegames Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agavegames, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: agavegames
provider_slug: agavegames
slug: agavegames-domain-security
source_filename: agavegames-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agavegames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agavegames.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agavegames/refs/heads/main/security/agavegames-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Mobile Games
- Puzzle Games
- Games
- Mobile
- Entertainment
---
