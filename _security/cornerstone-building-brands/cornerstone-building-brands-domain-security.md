---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cornerstonebuildingbrands.com
  spf: true
hosts:
- cert_expires: Sep 14 17:24:24 2026 GMT
  host: www.cornerstonebuildingbrands.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.cornerstonebuildingbrands.com
  https: false
- host: api.cornerstonebuildingbrands.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cornerstone Building Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cornerstone Building Brands, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cornerstone Building Brands
provider_slug: cornerstone-building-brands
slug: cornerstone-building-brands-domain-security
source_filename: cornerstone-building-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cornerstonebuildingbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:24:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.cornerstonebuildingbrands.com\n  https: false\n- host: api.cornerstonebuildingbrands.com\n  https: false\ndomains:\n- domain: cornerstonebuildingbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornerstone-building-brands/refs/heads/main/security/cornerstone-building-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Building Products
- Construction
---
