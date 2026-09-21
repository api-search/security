---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avonworldwide.com
  spf: false
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.avonworldwide.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avon Products Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avon Products, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Avon Products
provider_slug: avon-products
slug: avon-products-domain-security
source_filename: avon-products-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avonworldwide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: avonworldwide.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avon-products/refs/heads/main/security/avon-products-domain-security.yml
summary_line: TLSv1.3
tags:
- Fortune 500
- Beauty
- E-Commerce
- Retail
- Direct Sales
- Consumer Goods
---
