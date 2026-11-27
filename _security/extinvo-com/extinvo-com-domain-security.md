---
api_specs:
- filename: extinvo-com-dataset-api-openapi.yml
  format: yaml
  label: Extinvo Dataset API
  slug: extinvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extinvo-com/openapi/extinvo-com-dataset-api-openapi.yml
- filename: extinvo-com-mcp-api-openapi.yml
  format: yaml
  label: Extinvo MCP API
  slug: extinvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extinvo-com/openapi/extinvo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: extinvo.com
  spf: true
hosts:
- cert_expires: Feb  2 08:16:52 2027 GMT
  host: extinvo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Extinvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extinvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Extinvo
provider_slug: extinvo-com
slug: extinvo-com-domain-security
source_filename: extinvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extinvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 08:16:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: extinvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/extinvo-com/security/extinvo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fire Safety
- Inspection
- Software
- Tools
---
