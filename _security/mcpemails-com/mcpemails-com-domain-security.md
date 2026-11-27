---
api_specs:
- filename: mcpemails-com-openapi-generated.yml
  format: yaml
  label: MCP Emails API
  slug: mcpemails-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpemails-com/openapi/_ae-authored/mcpemails-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mcpemails.com
  spf: true
hosts:
- cert_expires: Dec 23 19:59:08 2026 GMT
  host: mcpemails.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Emails Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Emails, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MCP Emails
provider_slug: mcpemails-com
slug: mcpemails-com-domain-security
source_filename: mcpemails-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpemails.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 19:59:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpemails.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcpemails-com/security/mcpemails-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Artificial Intelligence
- MCP
- Cloud
- Services
---
