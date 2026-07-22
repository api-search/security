---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dealcart.io
  spf: false
hosts:
- cert_expires: Oct  7 18:46:24 2026 GMT
  host: dealcart.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealcart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealCart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DealCart
provider_slug: dealcart
slug: dealcart-domain-security
source_filename: dealcart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealcart.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:46:24 2026 GMT\n  hsts: false\ndomains:\n- domain: dealcart.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealcart/refs/heads/main/security/dealcart-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social Commerce
- E-Commerce
- Grocery
- Retail
- Pakistan
---
