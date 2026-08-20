---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pokkt.com
  spf: true
hosts:
- cert_expires: Oct  5 14:36:59 2026 GMT
  host: pokkt.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 02:50:45 2026 GMT
  host: wiki.pokkt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 06:57:40 2026 GMT
  host: vdo.pokkt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pokkt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pokkt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pokkt
provider_slug: pokkt
slug: pokkt-domain-security
source_filename: pokkt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: wiki.pokkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:50:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vdo.pokkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 06:57:40 2026 GMT\n  hsts: null\ndomains:\n- domain: pokkt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokkt/refs/heads/main/security/pokkt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Monetization
- Mobile
- Video Advertising
- AdTech
- Remarketing
- OpenRTB
- Programmatic Advertising
- Rewarded Video
- Mobile SDK
- Ad Serving
- Connected TV
- Supply Side Platform
- Demand-Side Platform
---
