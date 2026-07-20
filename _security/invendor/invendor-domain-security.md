---
api_specs:
- filename: invendor-common-openapi-original.json
  format: json
  label: Invendor Common API
  slug: invendor-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-common-openapi-original.json
- filename: invendor-reporting-openapi-original.json
  format: json
  label: Invendor Reporting API
  slug: invendor-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-reporting-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: invendor.com
  spf: true
hosts:
- cert_expires: Sep 24 13:09:27 2026 GMT
  host: invendor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Invendor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invendor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Invendor
provider_slug: invendor
slug: invendor-domain-security
source_filename: invendor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invendor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:09:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: invendor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/security/invendor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Inventory Management
- Vendor Managed Inventory
- Industrial Vending
- Supply Chain
- Warehouse Management
- Asset Tracking
---
