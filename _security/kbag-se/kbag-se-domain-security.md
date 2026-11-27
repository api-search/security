---
api_specs:
- filename: kbag-se-calculate-delivery-price-api-openapi.yml
  format: yaml
  label: K-Bag AB Calculate Delivery Price API
  slug: kbag-se-calculate-delivery-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kbag-se/openapi/kbag-se-calculate-delivery-price-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kbag.se
  spf: false
hosts:
- cert_expires: Feb  6 05:58:32 2027 GMT
  host: kbag.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: K-Bag AB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for K-Bag AB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: K-Bag AB
provider_slug: kbag-se
slug: kbag-se-domain-security
source_filename: kbag-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kbag.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 05:58:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kbag.se\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kbag-se/security/kbag-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Materials
- Waste-Pickup
- Sweden
---
