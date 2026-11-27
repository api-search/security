---
api_specs:
- filename: flatratebook-com-dataset-api-openapi.yml
  format: yaml
  label: FlatRateBook Dataset API
  slug: flatratebook-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatratebook-com/openapi/flatratebook-com-dataset-api-openapi.yml
- filename: flatratebook-com-mcp-api-openapi.yml
  format: yaml
  label: FlatRateBook MCP API
  slug: flatratebook-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatratebook-com/openapi/flatratebook-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flatratebook.com
  spf: true
hosts:
- cert_expires: Jan 30 16:17:09 2027 GMT
  host: flatratebook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlatRateBook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlatRateBook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FlatRateBook
provider_slug: flatratebook-com
slug: flatratebook-com-domain-security
source_filename: flatratebook-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatratebook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 16:17:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flatratebook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flatratebook-com/security/flatratebook-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Field Service Management
- Pricing
- Invoicing
- Calculator
- Small Business
---
