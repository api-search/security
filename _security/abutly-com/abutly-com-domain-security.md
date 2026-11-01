---
api_specs:
- filename: abutly-com-dataset-api-openapi.yml
  format: yaml
  label: abutly-com Dataset API
  slug: abutly-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abutly-com/openapi/abutly-com-dataset-api-openapi.yml
- filename: abutly-com-mcp-api-openapi.yml
  format: yaml
  label: abutly-com MCP API
  slug: abutly-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abutly-com/openapi/abutly-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abutly.com
  spf: true
hosts:
- cert_expires: Dec  4 09:18:23 2026 GMT
  host: abutly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abutly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for abutly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: abutly-com
provider_slug: abutly-com
slug: abutly-com-domain-security
source_filename: abutly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abutly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 09:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abutly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/abutly-com/security/abutly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Construction
- LegalTech
- PartyWall
- UK
---
