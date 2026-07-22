---
api_specs:
- filename: nory-middleware-openapi.json
  format: json
  label: Nory Middleware API
  slug: nory-middleware
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-middleware-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nory.ai
  spf: true
hosts:
- cert_expires: Sep 13 15:10:28 2026 GMT
  host: nory.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nory
provider_slug: nory
slug: nory-domain-security
source_filename: nory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:10:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nory.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/security/nory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurant
- Hospitality
- Inventory
- Workforce
- Payroll
- Point of Sale
- Artificial Intelligence
- Food and Beverage
---
