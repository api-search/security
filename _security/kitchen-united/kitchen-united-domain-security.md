---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kitchenunited.com
  spf: false
hosts:
- cert_expires: Oct  5 14:29:46 2026 GMT
  host: kitchenunited.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitchen United Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitchen United, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kitchen United
provider_slug: kitchen-united
slug: kitchen-united-domain-security
source_filename: kitchen-united-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitchenunited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kitchenunited.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitchen-united/refs/heads/main/security/kitchen-united-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Ghost Kitchens
- Restaurants
- Food Delivery
- Food Service
- Defunct
---
