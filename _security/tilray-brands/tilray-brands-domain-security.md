---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tilray.com
  spf: false
hosts:
- cert_expires: Aug 24 19:39:01 2026 GMT
  host: www.tilray.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tilray Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tilray Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Tilray Brands
provider_slug: tilray-brands
slug: tilray-brands-domain-security
source_filename: tilray-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tilray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:39:01 2026 GMT\n  hsts: false\ndomains:\n- domain: tilray.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tilray-brands/refs/heads/main/security/tilray-brands-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cannabis
- Beverages
- Wellness
- Consumer Packaged Goods
---
