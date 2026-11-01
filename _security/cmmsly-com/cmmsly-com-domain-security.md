---
api_specs:
- filename: cmmsly-com-dataset-api-openapi.yml
  format: yaml
  label: cmmsly-com Dataset API
  slug: cmmsly-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cmmsly-com/openapi/cmmsly-com-dataset-api-openapi.yml
- filename: cmmsly-com-mcp-api-openapi.yml
  format: yaml
  label: cmmsly-com MCP API
  slug: cmmsly-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cmmsly-com/openapi/cmmsly-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cmmsly.com
  spf: true
hosts:
- cert_expires: Dec  3 18:34:38 2026 GMT
  host: cmmsly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cmmsly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cmmsly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cmmsly-com
provider_slug: cmmsly-com
slug: cmmsly-com-domain-security
source_filename: cmmsly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cmmsly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 18:34:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cmmsly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cmmsly-com/security/cmmsly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CMMS
- Maintenance
- Equipment
- Software
- Tools
---
