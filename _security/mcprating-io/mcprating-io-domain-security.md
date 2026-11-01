---
api_specs:
- filename: mcprating-io-openapi-generated.yml
  format: yaml
  label: mcprating-io API
  slug: mcprating-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcprating-io/openapi/_ae-authored/mcprating-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcprating.io
  spf: true
hosts:
- cert_expires: Jan 18 00:39:00 2027 GMT
  host: mcprating.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcprating Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcprating-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mcprating-io
provider_slug: mcprating-io
slug: mcprating-io-domain-security
source_filename: mcprating-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcprating.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 00:39:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcprating.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcprating-io/security/mcprating-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- MCP
- Platform
- Catalog
- Security
---
