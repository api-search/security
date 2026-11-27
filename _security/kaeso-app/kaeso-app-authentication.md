---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: kaeso-app-agents-api-openapi.yml
  format: yaml
  label: Kaeso Agents API
  slug: kaeso-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-agents-api-openapi.yml
- filename: kaeso-app-auth-api-openapi.yml
  format: yaml
  label: Kaeso Auth API
  slug: kaeso-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-auth-api-openapi.yml
- filename: kaeso-app-instance-api-openapi.yml
  format: yaml
  label: Kaeso Instance API
  slug: kaeso-app-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-instance-api-openapi.yml
- filename: kaeso-app-logs-api-openapi.yml
  format: yaml
  label: Kaeso Logs API
  slug: kaeso-app-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-logs-api-openapi.yml
- filename: kaeso-app-me-api-openapi.yml
  format: yaml
  label: Kaeso Me API
  slug: kaeso-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-me-api-openapi.yml
- filename: kaeso-app-models-api-openapi.yml
  format: yaml
  label: Kaeso Models API
  slug: kaeso-app-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-models-api-openapi.yml
- filename: kaeso-app-orgs-api-openapi.yml
  format: yaml
  label: Kaeso Orgs API
  slug: kaeso-app-orgs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-orgs-api-openapi.yml
- filename: kaeso-app-projects-api-openapi.yml
  format: yaml
  label: Kaeso Projects API
  slug: kaeso-app-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-projects-api-openapi.yml
- filename: kaeso-app-response-cache-api-openapi.yml
  format: yaml
  label: Kaeso Response Cache API
  slug: kaeso-app-response-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-response-cache-api-openapi.yml
- filename: kaeso-app-stored-responses-api-openapi.yml
  format: yaml
  label: Kaeso Stored Responses API
  slug: kaeso-app-stored-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaeso-app/openapi/kaeso-app-stored-responses-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Kaeso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaeso secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kaeso
provider_slug: kaeso-app
scheme_count: 2
schemes:
- description: An agent's access token (`kso_at_…`) from the OAuth sign-in of the MCP server at `/mcp`. The agent acts for its user with the rights both hold, within the instance's and each org's agent policies.
  name: agent
  scheme: bearer
  sources:
  - openapi/kaeso-app-openapi.json
  type: http
- description: The console session cookie, set by the sign-in endpoints. Every request other than `GET`, `HEAD` and `OPTIONS` that carries it, and every such request to a public `auth/*` endpoint, must also send `Origin` with the origin of the install's public URL; `orgs/{org}/*` requests with an API key need none.
  in: cookie
  name: session
  parameter: __Host-kaeso_session
  sources:
  - openapi/kaeso-app-openapi.json
  type: apiKey
slug: kaeso-app-authentication
source_filename: kaeso-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/kaeso-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: agent\n  type: http\n  scheme: bearer\n  description: An agent's access token (`kso_at_…`) from the OAuth sign-in of the MCP server\n    at `/mcp`. The agent acts for its user with the rights both hold, within the instance's\n    and each org's agent policies.\n  sources:\n  - openapi/kaeso-app-openapi.json\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: __Host-kaeso_session\n  description: The console session cookie, set by the sign-in endpoints. Every request other\n    than `GET`, `HEAD` and `OPTIONS` that carries it, and every such request to a public `auth/*`\n    endpoint, must also send `Origin` with the origin of the install's public URL; `orgs/{org}/*`\n    requests with an API key need none.\n  sources:\n  - openapi/kaeso-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kaeso-app/authentication/kaeso-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Open Source
- Rust
- Self-Hosted
- Gateways
- LLM
---
