---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voodoo.io
  spf: true
hosts:
- cert_expires: Oct 13 10:06:10 2026 GMT
  host: voodoo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: v2-publidash-api.voodoo.io
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Voodoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voodoo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voodoo
provider_slug: voodoo
slug: voodoo-domain-security
source_filename: voodoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voodoo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:06:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: v2-publidash-api.voodoo.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: voodoo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voodoo/refs/heads/main/security/voodoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Mobile Games
- Mobile Apps
- Advertising
- Ad Network
- Game Publishing
- Mobile SDK
- Monetization
- Social Apps
---
