---
api_specs:
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Tool Router API
  slug: tool-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Tools API
  slug: tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Connected Accounts API
  slug: connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Auth Configs API
  slug: auth-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Toolkits API
  slug: toolkits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio MCP API
  slug: mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
- filename: composio-openapi-original.yml
  format: yaml
  label: Composio Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-openapi-original.yml
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
- Integrations
- MCP
- OAuth
- Sandbox
- Tools
- Triggers
- Unified_API
- Webhooks
---
