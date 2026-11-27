---
api_specs:
- filename: exitvo-com-dataset-api-openapi.yml
  format: yaml
  label: Exitvo Dataset API
  slug: exitvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvo-com/openapi/exitvo-com-dataset-api-openapi.yml
- filename: exitvo-com-mcp-api-openapi.yml
  format: yaml
  label: Exitvo MCP API
  slug: exitvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvo-com/openapi/exitvo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: exitvo.com
  spf: true
hosts:
- cert_expires: Jan 31 23:36:40 2027 GMT
  host: exitvo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exitvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exitvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Exitvo
provider_slug: exitvo-com
slug: exitvo-com-domain-security
source_filename: exitvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exitvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:36:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exitvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/exitvo-com/security/exitvo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Business
- Tools
- Checklist
- Valuation
---
