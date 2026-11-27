---
api_specs:
- filename: fitouto-com-dataset-api-openapi.yml
  format: yaml
  label: Fitouto Dataset API
  slug: fitouto-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fitouto-com/openapi/fitouto-com-dataset-api-openapi.yml
- filename: fitouto-com-mcp-api-openapi.yml
  format: yaml
  label: Fitouto MCP API
  slug: fitouto-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fitouto-com/openapi/fitouto-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fitouto.com
  spf: true
hosts:
- cert_expires: Feb  1 05:05:51 2027 GMT
  host: fitouto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fitouto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fitouto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fitouto
provider_slug: fitouto-com
slug: fitouto-com-domain-security
source_filename: fitouto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fitouto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 05:05:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fitouto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fitouto-com/security/fitouto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Office
- Management
- Software-as-a-Service
- Paperless
- Small Business
---
