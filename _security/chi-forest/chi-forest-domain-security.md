---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chiforest.com
  spf: true
hosts:
- cert_expires: Oct  9 07:50:14 2026 GMT
  host: www.chiforest.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chi Forest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chi Forest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chi Forest
provider_slug: chi-forest
slug: chi-forest-domain-security
source_filename: chi-forest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chiforest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:50:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: chiforest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chi-forest/refs/heads/main/security/chi-forest-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Beverages
- Food and Beverage
- Sparkling Water
- Direct to Consumer
- Retail
- Consumer Packaged Goods
---
