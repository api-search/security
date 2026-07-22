---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avon-products.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avon.com
  spf: true
hosts:
- cert_expires: Aug 13 20:19:26 2026 GMT
  host: www.avon-products.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.avon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Avon Products Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avon Products, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avon Products
provider_slug: avon-products
slug: avon-products-domain-security
source_filename: avon-products-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avon-products.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 20:19:26 2026 GMT\n  hsts: false\n- host: developer.avon.com\n  https: false\ndomains:\n- domain: avon-products.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: avon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avon-products/refs/heads/main/security/avon-products-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
- Beauty
- E-Commerce
- Retail
- Direct Sales
- Consumer Goods
---
