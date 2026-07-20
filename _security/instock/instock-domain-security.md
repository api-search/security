---
api_specs:
- filename: instock-openapi.json
  format: json
  label: Instock API
  slug: instock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instock/refs/heads/main/openapi/instock-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: instock.com
  spf: true
hosts:
- cert_expires: Aug 10 12:54:21 2026 GMT
  host: instock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 12:54:21 2026 GMT
  host: api.instock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Instock
provider_slug: instock
slug: instock-domain-security
source_filename: instock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:54:21 2026 GMT\n  hsts: false\n- host: api.instock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:54:21 2026 GMT\n  hsts: null\ndomains:\n- domain: instock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instock/refs/heads/main/security/instock-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Warehouse Automation
- Fulfillment
- Logistics
- ASRS
- Supply Chain
- Inventory Management
---
