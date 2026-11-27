---
api_specs:
- filename: eposvo-com-dataset-api-openapi.yml
  format: yaml
  label: Eposvo Dataset API
  slug: eposvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eposvo-com/openapi/eposvo-com-dataset-api-openapi.yml
- filename: eposvo-com-mcp-api-openapi.yml
  format: yaml
  label: Eposvo MCP API
  slug: eposvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eposvo-com/openapi/eposvo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eposvo.com
  spf: true
hosts:
- cert_expires: Feb  2 07:11:46 2027 GMT
  host: eposvo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eposvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eposvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eposvo
provider_slug: eposvo-com
slug: eposvo-com-domain-security
source_filename: eposvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eposvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 07:11:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eposvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/eposvo-com/security/eposvo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- EPOS
- Restaurant
- United Kingdom
- Software-as-a-Service
---
