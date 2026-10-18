---
api_specs:
- filename: tembo-agents-api-openapi.yml
  format: yaml
  label: Tembo Agents API
  slug: tembo-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-agents-api-openapi.yml
- filename: tembo-api-keys-api-openapi.yml
  format: yaml
  label: Tembo API Keys API
  slug: tembo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-api-keys-api-openapi.yml
- filename: tembo-artifacts-api-openapi.yml
  format: yaml
  label: Tembo Artifacts API
  slug: tembo-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-artifacts-api-openapi.yml
- filename: tembo-authentication-api-openapi.yml
  format: yaml
  label: Tembo Authentication API
  slug: tembo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-authentication-api-openapi.yml
- filename: tembo-billing-api-openapi.yml
  format: yaml
  label: Tembo Billing API
  slug: tembo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-billing-api-openapi.yml
- filename: tembo-insights-api-openapi.yml
  format: yaml
  label: Tembo Insights API
  slug: tembo-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-insights-api-openapi.yml
- filename: tembo-integrations-api-openapi.yml
  format: yaml
  label: Tembo Integrations API
  slug: tembo-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-integrations-api-openapi.yml
- filename: tembo-mcp-connections-api-openapi.yml
  format: yaml
  label: Tembo MCP Connections API
  slug: tembo-mcp-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-mcp-connections-api-openapi.yml
- filename: tembo-messages-api-openapi.yml
  format: yaml
  label: Tembo Messages API
  slug: tembo-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-messages-api-openapi.yml
- filename: tembo-models-api-openapi.yml
  format: yaml
  label: Tembo Models API
  slug: tembo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-models-api-openapi.yml
- filename: tembo-oauth-api-openapi.yml
  format: yaml
  label: Tembo OAuth API
  slug: tembo-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-oauth-api-openapi.yml
- filename: tembo-organizations-api-openapi.yml
  format: yaml
  label: Tembo Organizations API
  slug: tembo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-organizations-api-openapi.yml
- filename: tembo-projects-api-openapi.yml
  format: yaml
  label: Tembo Projects API
  slug: tembo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-projects-api-openapi.yml
- filename: tembo-pull-requests-api-openapi.yml
  format: yaml
  label: Tembo Pull requests API
  slug: tembo-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-pull-requests-api-openapi.yml
- filename: tembo-repositories-api-openapi.yml
  format: yaml
  label: Tembo Repositories API
  slug: tembo-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-repositories-api-openapi.yml
- filename: tembo-runtimes-api-openapi.yml
  format: yaml
  label: Tembo Runtimes API
  slug: tembo-runtimes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-runtimes-api-openapi.yml
- filename: tembo-sessions-api-openapi.yml
  format: yaml
  label: Tembo Sessions API
  slug: tembo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-sessions-api-openapi.yml
- filename: tembo-skills-api-openapi.yml
  format: yaml
  label: Tembo Skills API
  slug: tembo-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-skills-api-openapi.yml
- filename: tembo-users-api-openapi.yml
  format: yaml
  label: Tembo Users API
  slug: tembo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tembo.io
  spf: true
hosts:
- cert_expires: Dec  7 12:23:25 2026 GMT
  host: tembo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tembo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tembo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tembo
provider_slug: tembo
slug: tembo-domain-security
source_filename: tembo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tembo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 12:23:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tembo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/security/tembo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Coding Agents
- Developer Tools
- Sandbox
- MCP
- Automation
---
