---
api_specs:
- filename: composio-auth-configs-api-openapi.yml
  format: yaml
  label: Composio Auth Configs API
  slug: composio-auth-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-auth-configs-api-openapi.yml
- filename: composio-authentication-api-openapi.yml
  format: yaml
  label: Composio Authentication API
  slug: composio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-authentication-api-openapi.yml
- filename: composio-cli-api-openapi.yml
  format: yaml
  label: Composio CLI API
  slug: composio-cli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-cli-api-openapi.yml
- filename: composio-cli-authentication-api-openapi.yml
  format: yaml
  label: Composio CLI Authentication API
  slug: composio-cli-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-cli-authentication-api-openapi.yml
- filename: composio-connected-accounts-api-openapi.yml
  format: yaml
  label: Composio Connected Accounts API
  slug: composio-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-connected-accounts-api-openapi.yml
- filename: composio-files-api-openapi.yml
  format: yaml
  label: Composio Files API
  slug: composio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-files-api-openapi.yml
- filename: composio-logs-api-openapi.yml
  format: yaml
  label: Composio Logs API
  slug: composio-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-logs-api-openapi.yml
- filename: composio-mcp-api-openapi.yml
  format: yaml
  label: Composio MCP API
  slug: composio-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-mcp-api-openapi.yml
- filename: composio-migration-api-openapi.yml
  format: yaml
  label: Composio Migration API
  slug: composio-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-migration-api-openapi.yml
- filename: composio-organization-management-api-openapi.yml
  format: yaml
  label: Composio Organization Management API
  slug: composio-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-organization-management-api-openapi.yml
- filename: composio-projects-api-openapi.yml
  format: yaml
  label: Composio Projects API
  slug: composio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-projects-api-openapi.yml
- filename: composio-tool-router-api-openapi.yml
  format: yaml
  label: Composio Tool Router API
  slug: composio-tool-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-tool-router-api-openapi.yml
- filename: composio-toolkits-api-openapi.yml
  format: yaml
  label: Composio Toolkits API
  slug: composio-toolkits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-toolkits-api-openapi.yml
- filename: composio-tools-api-openapi.yml
  format: yaml
  label: Composio Tools API
  slug: composio-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-tools-api-openapi.yml
- filename: composio-triggers-api-openapi.yml
  format: yaml
  label: Composio Triggers API
  slug: composio-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-triggers-api-openapi.yml
- filename: composio-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Composio Webhook Endpoints API
  slug: composio-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-webhook-endpoints-api-openapi.yml
- filename: composio-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Composio Webhook Subscriptions API
  slug: composio-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: composio.dev
  spf: true
hosts:
- cert_expires: Oct  2 04:56:52 2026 GMT
  host: app.composio.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:43:01 2026 GMT
  host: docs.composio.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 04:56:52 2026 GMT
  host: backend.composio.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Composio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Composio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Composio
provider_slug: composio
slug: composio-domain-security
source_filename: composio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.composio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.composio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:43:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: backend.composio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: composio.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/security/composio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Authentication
- Integration
- MCP
- Sandbox
- Tools
- Triggers
- Unified-API
- Webhook
---
