---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: playerslounge.com
  spf: true
hosts:
- cert_expires: Sep 21 23:44:21 2026 GMT
  host: www.playerslounge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Players Lounge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Players Lounge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Players Lounge
provider_slug: players-lounge
slug: players-lounge-domain-security
source_filename: players-lounge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playerslounge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:44:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: playerslounge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/players-lounge/refs/heads/main/security/players-lounge-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Esports
- Skill-Based Gaming
- Money Matches
- Player Staking
- Consumer
- Video Games
---
