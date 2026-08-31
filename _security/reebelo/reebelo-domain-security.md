---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reebelo.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: reebelo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: cobalt.reebelo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: a.reebelo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reebelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reebelo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reebelo
provider_slug: reebelo
slug: reebelo-domain-security
source_filename: reebelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reebelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cobalt.reebelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: a.reebelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reebelo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reebelo/refs/heads/main/security/reebelo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Refurbished Electronics
- Marketplace
- E-Commerce
- Consumer Electronics
- Reverse Logistics
- Circular Economy
- Retail
- Inventory
- Order
- Seller Integration
---
