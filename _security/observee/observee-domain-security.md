---
api_specs:
- filename: observee-plants-api-openapi.yml
  format: yaml
  label: Observee MCP API
  slug: observee-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/observee/openapi/observee-plants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: observee.ai
  spf: true
hosts:
- cert_expires: Dec 29 16:37:55 2026 GMT
  host: observee.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Observee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Observee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Observee
provider_slug: observee
slug: observee-domain-security
source_filename: observee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: observee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 16:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: observee.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/observee/security/observee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- MCP
- Integration
- Observability
- Platform
---
