---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: abiosgaming.com
  spf: true
hosts:
- cert_expires: Sep 20 12:40:10 2026 GMT
  host: abiosgaming.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: atlas.abiosgaming.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Abios Gaming Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abios (Sportradar), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Abios (Sportradar)
provider_slug: abios-gaming
slug: abios-gaming-domain-security
source_filename: abios-gaming-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abiosgaming.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:40:10 2026 GMT\n  hsts: false\n- host: atlas.abiosgaming.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: abiosgaming.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abios-gaming/refs/heads/main/security/abios-gaming-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Esports
- Sports Data
- Odds
- Widgets
- Live Data
- WebSocket
- REST
- Sportradar
---
