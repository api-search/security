---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: noon.com
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: www.noon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Noon
provider_slug: noon
slug: noon-domain-security
source_filename: noon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: noon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noon/refs/heads/main/security/noon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Marketplace
- Retail
- Online Shopping
- MENA
- Middle East
- United Arab Emirates
- Saudi Arabia
- Egypt
- Dubai
- Sellers
- Food Delivery
- Q-Commerce
- Grocery Delivery
- Payments
- Digital Wallet
- Logistics
- Last-Mile Delivery
- Super App
---
