---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toryburch.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.toryburch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tory Burch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tory Burch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tory Burch
provider_slug: tory-burch
slug: tory-burch-domain-security
source_filename: tory-burch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toryburch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toryburch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tory-burch/refs/heads/main/security/tory-burch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Luxury Goods
- Apparel
- Footwear
- Handbags and Accessories
- Retail
- Ecommerce
- Direct to Consumer
- Consumer Brands
- United States
---
