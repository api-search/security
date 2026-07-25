---
api_specs:
- filename: integration-app-actions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Actions API
  slug: integration-app-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-actions-api-openapi.yml
- filename: integration-app-app-event-subscriptions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) App Event Subscriptions API
  slug: integration-app-app-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-app-event-subscriptions-api-openapi.yml
- filename: integration-app-connections-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Connections API
  slug: integration-app-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-connections-api-openapi.yml
- filename: integration-app-connectors-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Connectors API
  slug: integration-app-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-connectors-api-openapi.yml
- filename: integration-app-customers-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Customers API
  slug: integration-app-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-customers-api-openapi.yml
- filename: integration-app-data-collections-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Data Collections API
  slug: integration-app-data-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-data-collections-api-openapi.yml
- filename: integration-app-external-event-subscriptions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) External Event Subscriptions API
  slug: integration-app-external-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-external-event-subscriptions-api-openapi.yml
- filename: integration-app-field-mappings-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Field Mappings API
  slug: integration-app-field-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-field-mappings-api-openapi.yml
- filename: integration-app-flow-runs-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Flow Runs API
  slug: integration-app-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-flow-runs-api-openapi.yml
- filename: integration-app-flows-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Flows API
  slug: integration-app-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-flows-api-openapi.yml
- filename: integration-app-integrations-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Integrations API
  slug: integration-app-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-integrations-api-openapi.yml
- filename: integration-app-logs-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Logs API
  slug: integration-app-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-logs-api-openapi.yml
- filename: integration-app-public-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Public API
  slug: integration-app-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-public-api-openapi.yml
- filename: integration-app-search-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Search API
  slug: integration-app-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-search-api-openapi.yml
- filename: integration-app-sessions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Sessions API
  slug: integration-app-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getmembrane.com
  spf: true
hosts:
- cert_expires: Oct  9 12:56:08 2026 GMT
  host: getmembrane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 12:56:08 2026 GMT
  host: api.getmembrane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integration App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integration.app (Membrane), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Integration.app (Membrane)
provider_slug: integration-app
slug: integration-app-domain-security
source_filename: integration-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmembrane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:56:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getmembrane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:56:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmembrane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/security/integration-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic Integrations
- AI Agents
- Connectors
- Embedded Integrations
- Embedded iPaaS
- Integration Marketplace
- MCP
- Model Context Protocol
- Self-Hosting
- Unified API
---
