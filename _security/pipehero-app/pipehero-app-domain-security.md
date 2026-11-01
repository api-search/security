---
api_specs:
- filename: pipehero-app-mcp-api-openapi.yml
  format: yaml
  label: pipehero-app MCP API
  slug: pipehero-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-mcp-api-openapi.yml
- filename: pipehero-app-slack-api-openapi.yml
  format: yaml
  label: pipehero-app Slack API
  slug: pipehero-app-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-slack-api-openapi.yml
- filename: pipehero-app-webhooks-api-openapi.yml
  format: yaml
  label: pipehero-app Webhooks API
  slug: pipehero-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pipehero.app
  spf: true
hosts:
- cert_expires: Dec  6 05:22:54 2026 GMT
  host: pipehero.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pipehero App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pipehero-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: pipehero-app
provider_slug: pipehero-app
slug: pipehero-app-domain-security
source_filename: pipehero-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pipehero.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 05:22:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pipehero.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pipehero-app/security/pipehero-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Webhook
- API Workspace
- Developer Tools
- MCP
- Integration
---
