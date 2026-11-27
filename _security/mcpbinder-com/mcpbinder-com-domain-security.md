---
api_specs:
- filename: mcpbinder-com-openapi-generated.yml
  format: yaml
  label: MCPBinder API
  slug: mcpbinder-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpbinder-com/openapi/_ae-authored/mcpbinder-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpbinder.com
  spf: true
hosts:
- cert_expires: Dec 26 15:24:17 2026 GMT
  host: mcpbinder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPBinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPBinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MCPBinder
provider_slug: mcpbinder-com
slug: mcpbinder-com-domain-security
source_filename: mcpbinder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpbinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:24:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpbinder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcpbinder-com/security/mcpbinder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workspace
- AI Agent Integration
---
