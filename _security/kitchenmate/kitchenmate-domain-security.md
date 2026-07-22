---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kitchenmate.com
  spf: true
hosts:
- cert_expires: Sep  1 02:30:43 2026 GMT
  host: kitchenmate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitchenmate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KitchenMate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KitchenMate
provider_slug: kitchenmate
slug: kitchenmate-domain-security
source_filename: kitchenmate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitchenmate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:30:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kitchenmate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitchenmate/refs/heads/main/security/kitchenmate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Autonomous Retail
- Vending
- Smart Devices
- Internet of Things
- Workplace Services
- Hardware
---
