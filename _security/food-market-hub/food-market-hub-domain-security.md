---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foodmarkethub.com
  spf: true
hosts:
- cert_expires: Aug  2 01:12:52 2026 GMT
  host: foodmarkethub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Food Market Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Food Market Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Food Market Hub
provider_slug: food-market-hub
slug: food-market-hub-domain-security
source_filename: food-market-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foodmarkethub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 01:12:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foodmarkethub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-market-hub/refs/heads/main/security/food-market-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Restaurants
- Supply Chain
- Procurement
- Inventory Management
- Hospitality
- SaaS
- Southeast Asia
---
