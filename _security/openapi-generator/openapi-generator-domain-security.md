---
api_specs:
- filename: openapi-generator-clients-api-openapi.yml
  format: yaml
  label: OpenAPI Generator Clients API
  slug: openapi-generator-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/openapi/openapi-generator-clients-api-openapi.yml
- filename: openapi-generator-servers-api-openapi.yml
  format: yaml
  label: OpenAPI Generator Servers API
  slug: openapi-generator-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/openapi/openapi-generator-servers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openapi-generator.tech
  spf: false
hosts:
- cert_expires: Sep 29 11:13:19 2026 GMT
  host: openapi-generator.tech
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 16:28:51 2026 GMT
  host: api.openapi-generator.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openapi Generator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAPI Generator, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenAPI Generator
provider_slug: openapi-generator
slug: openapi-generator-domain-security
source_filename: openapi-generator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openapi-generator.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.openapi-generator.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 16:28:51 2026 GMT\n  hsts: false\ndomains:\n- domain: openapi-generator.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/security/openapi-generator-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Code Generation
- Documentation
- Open-Source
- OpenAPI
- SDK
- API Tooling
- Developer Tools
- Swagger
- Server Stubs
- Codegen
---
