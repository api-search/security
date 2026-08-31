---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: truff.com
  spf: true
hosts:
- cert_expires: Nov 28 06:12:32 2026 GMT
  host: www.truff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 20:13:03 2026 GMT
  host: shop.truff.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRUFF, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TRUFF
provider_slug: truff
slug: truff-domain-security
source_filename: truff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 06:12:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.truff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 20:13:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: truff.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truff/refs/heads/main/security/truff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Condiments
- Direct to Consumer
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Shopify
---
