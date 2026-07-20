---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: freshop.com
  spf: true
hosts:
- cert_expires: Sep  2 03:48:59 2026 GMT
  host: freshop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Freshop
provider_slug: freshop
slug: freshop-domain-security
source_filename: freshop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshop/refs/heads/main/security/freshop-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Grocery
- eCommerce
- Retail
- Online Shopping
- Fulfillment
- Delivery
- NCR Voyix
---
