---
api_specs:
- filename: farmers-edge-farmcommand-openapi-original.json
  format: json
  label: FarmCommand API
  slug: farmcommand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-farmcommand-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: farmcommand.com
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.farmcommand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: developer.farmcommand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: admin.farmcommand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmers Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Edge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Farmers Edge
provider_slug: farmers-edge
slug: farmers-edge-domain-security
source_filename: farmers-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: admin.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmcommand.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/security/farmers-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- Agriculture
- Precision Agriculture
- AgTech
- Farm Management
- Digital Agriculture
- IoT
- Weather
- Carbon
- API
---
