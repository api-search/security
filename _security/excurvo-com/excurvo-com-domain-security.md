---
api_specs:
- filename: excurvo-com-dataset-api-openapi.yml
  format: yaml
  label: Excurvo Dataset API
  slug: excurvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/excurvo-com/openapi/excurvo-com-dataset-api-openapi.yml
- filename: excurvo-com-mcp-api-openapi.yml
  format: yaml
  label: Excurvo MCP API
  slug: excurvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/excurvo-com/openapi/excurvo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: excurvo.com
  spf: true
hosts:
- cert_expires: Feb  2 08:00:44 2027 GMT
  host: excurvo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Excurvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Excurvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Excurvo
provider_slug: excurvo-com
slug: excurvo-com-domain-security
source_filename: excurvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: excurvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 08:00:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: excurvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/excurvo-com/security/excurvo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Travel
- Booking
- Software-as-a-Service
- Tours
- Tools
---
