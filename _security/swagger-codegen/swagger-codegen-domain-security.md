---
api_specs:
- filename: swagger-generator-openapi.yml
  format: yaml
  label: Swagger Generator API
  slug: swagger-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-generator-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swagger.io
  spf: true
hosts:
- cert_expires: Oct  4 16:46:01 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: generator3.swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Swagger Codegen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swagger Codegen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swagger Codegen
provider_slug: swagger-codegen
slug: swagger-codegen-domain-security
source_filename: swagger-codegen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:46:01 2026 GMT\n  hsts: false\n- host: generator3.swagger.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: swagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/security/swagger-codegen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Client Libraries
- Code Generation
- Open Source
- OpenAPI
- SDK
---
