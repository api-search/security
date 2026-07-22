---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peak.com
  spf: true
hosts:
- cert_expires: Oct 14 08:44:21 2026 GMT
  host: peak.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peak Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peak Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peak Games
provider_slug: peak-games
slug: peak-games-domain-security
source_filename: peak-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:44:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: peak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peak-games/refs/heads/main/security/peak-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Mobile Games
- Game Development
- Entertainment
- Casual Games
---
