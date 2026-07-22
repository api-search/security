---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stylesaint.com
  spf: false
hosts:
- cert_expires: Aug 27 13:36:31 2026 GMT
  host: stylesaint.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stylesaint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StyleSaint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: StyleSaint
provider_slug: stylesaint
slug: stylesaint-domain-security
source_filename: stylesaint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stylesaint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: stylesaint.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stylesaint/refs/heads/main/security/stylesaint-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fashion
- Ecommerce
- Retail
- Apparel
- Direct to Consumer
- Shopify
---
