---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conagrabrands.com
  spf: false
hosts:
- cert_expires: Aug  2 21:23:57 2026 GMT
  host: www.conagrabrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conagra Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conagra Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Conagra Brands
provider_slug: conagra-brands
slug: conagra-brands-domain-security
source_filename: conagra-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conagrabrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 21:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conagrabrands.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conagra-brands/refs/heads/main/security/conagra-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Branded Foods
- CPG
- Consumer Packaged Goods
- Foodservice
- Fortune 500
- Frozen Foods
- Grocery
---
