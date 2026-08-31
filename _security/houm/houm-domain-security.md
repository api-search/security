---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: houm.com
  spf: true
hosts:
- cert_expires: Sep 21 21:11:43 2026 GMT
  host: houm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Houm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Houm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Houm
provider_slug: houm
slug: houm-domain-security
source_filename: houm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: houm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:11:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: houm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houm/refs/heads/main/security/houm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- PropTech
- Property Management
- Rentals
- Marketplace
- Latin America
- Chile
- Mexico
- Colombia
---
