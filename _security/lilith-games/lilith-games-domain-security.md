---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lilith.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.lilith.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lilith Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilith Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lilith Games
provider_slug: lilith-games
slug: lilith-games-domain-security
source_filename: lilith-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lilith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lilith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilith-games/refs/heads/main/security/lilith-games-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Video Games
- Game Development
- Game Publishing
- Mobile Games
- Entertainment
- China
---
