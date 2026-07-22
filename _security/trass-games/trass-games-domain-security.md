---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trass.games
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: yeeps.com
  spf: false
hosts:
- cert_expires: Sep 19 12:18:47 2026 GMT
  host: trass.games
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:42:32 2026 GMT
  host: yeeps.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trass Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trass Games, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trass Games
provider_slug: trass-games
slug: trass-games-domain-security
source_filename: trass-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trass.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:18:47 2026 GMT\n  hsts: false\n- host: yeeps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:42:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: trass.games\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: yeeps.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trass-games/refs/heads/main/security/trass-games-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Gaming
- Virtual Reality
- VR Games
- Meta Quest
- Social Games
- Ecommerce
- Entertainment
---
