---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getgorgie.com
  spf: true
hosts:
- cert_expires: Sep  8 15:41:03 2026 GMT
  host: getgorgie.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gorgie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GORGIE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GORGIE
provider_slug: gorgie
slug: gorgie-domain-security
source_filename: gorgie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getgorgie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:41:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: getgorgie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorgie/refs/heads/main/security/gorgie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Consumer Packaged Goods
- Energy Drink
- Beverage
- Wellness
- Ecommerce
- Direct to Consumer
---
