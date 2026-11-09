---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: countrydelight.in
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: www.countrydelight.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Countrydelight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Country Delight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Country Delight
provider_slug: countrydelight
slug: countrydelight-domain-security
source_filename: countrydelight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.countrydelight.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: countrydelight.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/countrydelight/security/countrydelight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Grocery Delivery
- Dairy
- Milk
- Direct to Consumer
- Consumer
- Food and Beverage
- Subscription
- India
- Consumer Goods
---
