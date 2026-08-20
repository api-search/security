---
api_key_in: []
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
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Integration App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Integration.app (Membrane) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Integration.app (Membrane)
provider_slug: integration-app
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer token in the Authorization header. Test tokens are available

    from workspace settings; admin-level tokens are required for

    administrative operations.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/integration-app-openapi.yml
  type: http
slug: integration-app-authentication
source_filename: integration-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/integration-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Bearer token in the Authorization header. Test tokens are available\n    from workspace settings; admin-level tokens are required for\n    administrative operations.\n  sources:\n  - openapi/integration-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/authentication/integration-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Agentic Integrations
- AI Agents
- Connectors
- Embedded Integrations
- Embedded iPaaS
- Integration Marketplace
- MCP
- Self-Hosting
- Unified-API
---
