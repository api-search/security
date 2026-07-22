---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centricbrands.com
  spf: true
hosts:
- cert_expires: Sep 22 12:19:51 2026 GMT
  host: www.centricbrands.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centric Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centric Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Centric Brands
provider_slug: centric-brands
slug: centric-brands-domain-security
source_filename: centric-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centricbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:19:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: centricbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centric-brands/refs/heads/main/security/centric-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Accessories
- Footwear
- Beauty
- Kids
- Lifestyle
- Brand Management
- Licensing
- Entertainment Licensing
- Sports Licensing
- Fashion
- Consumer Products
- Fortune 1000
- Private Equity Owned
---
