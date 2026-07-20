---
api_specs:
- filename: deliverart-openapi.yml
  format: yaml
  label: Deliverart API
  slug: deliverart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deliverart.it
  spf: true
hosts:
- cert_expires: Sep 29 12:42:10 2026 GMT
  host: deliverart.it
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: pubapi.deliverart.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deliverart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deliverart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deliverart
provider_slug: deliverart
slug: deliverart-domain-security
source_filename: deliverart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deliverart.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:42:10 2026 GMT\n  hsts: false\n- host: pubapi.deliverart.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deliverart.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/security/deliverart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
---
