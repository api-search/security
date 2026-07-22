---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swiperxapp.com
  spf: true
hosts:
- cert_expires: Aug 22 08:16:01 2026 GMT
  host: swiperxapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiperx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwipeRx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SwipeRx
provider_slug: swiperx
slug: swiperx-domain-security
source_filename: swiperx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swiperxapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:16:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swiperxapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiperx/refs/heads/main/security/swiperx-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Pharmacy
- B2B Commerce
- E-commerce
- Southeast Asia
- Marketplace
- Digital Health
- Mobile
---
