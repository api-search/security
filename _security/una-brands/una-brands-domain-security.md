---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: una-brands.com
  spf: true
hosts:
- cert_expires: Sep  6 04:59:32 2026 GMT
  host: una-brands.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Una Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Una Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Una Brands
provider_slug: una-brands
slug: una-brands-domain-security
source_filename: una-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: una-brands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:59:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: una-brands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/una-brands/refs/heads/main/security/una-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- eCommerce
- House of Brands
- Brand Aggregator
- Consumer Goods
- Retail
- Singapore
- APAC
---
