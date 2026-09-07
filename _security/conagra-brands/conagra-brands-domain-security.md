---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conagrabrands.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conagrafoods.com
  spf: true
hosts:
- cert_expires: Oct 12 03:26:32 2026 GMT
  host: www.conagrabrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: brands-api.conagrafoods.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Conagra Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conagra Brands, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Conagra Brands
provider_slug: conagra-brands
slug: conagra-brands-domain-security
source_filename: conagra-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conagrabrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:26:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: brands-api.conagrafoods.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: conagrabrands.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: conagrafoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conagra-brands/refs/heads/main/security/conagra-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Branded Foods
- CPG
- Consumer Packaged Goods
- Food Service
- Fortune 500
- Frozen Foods
- Grocery
- OData
- Product Data
---
