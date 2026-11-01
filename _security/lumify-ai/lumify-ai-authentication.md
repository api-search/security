---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumify-ai-admin-api-openapi.yml
  format: yaml
  label: lumify-ai Admin API
  slug: lumify-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-admin-api-openapi.yml
- filename: lumify-ai-agent-api-openapi.yml
  format: yaml
  label: lumify-ai Agent API
  slug: lumify-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-agent-api-openapi.yml
- filename: lumify-ai-app-api-openapi.yml
  format: yaml
  label: lumify-ai App API
  slug: lumify-ai-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-app-api-openapi.yml
- filename: lumify-ai-auth-api-openapi.yml
  format: yaml
  label: lumify-ai Auth API
  slug: lumify-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-auth-api-openapi.yml
- filename: lumify-ai-events-api-openapi.yml
  format: yaml
  label: lumify-ai Events API
  slug: lumify-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-events-api-openapi.yml
- filename: lumify-ai-grade-api-openapi.yml
  format: yaml
  label: lumify-ai Grade API
  slug: lumify-ai-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-grade-api-openapi.yml
- filename: lumify-ai-health-api-openapi.yml
  format: yaml
  label: lumify-ai Health API
  slug: lumify-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-health-api-openapi.yml
- filename: lumify-ai-mcp-api-openapi.yml
  format: yaml
  label: lumify-ai MCP API
  slug: lumify-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-mcp-api-openapi.yml
- filename: lumify-ai-oauth-api-openapi.yml
  format: yaml
  label: lumify-ai OAuth API
  slug: lumify-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-oauth-api-openapi.yml
- filename: lumify-ai-players-api-openapi.yml
  format: yaml
  label: lumify-ai Players API
  slug: lumify-ai-players-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-players-api-openapi.yml
- filename: lumify-ai-public-api-openapi.yml
  format: yaml
  label: lumify-ai Public API
  slug: lumify-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-public-api-openapi.yml
- filename: lumify-ai-resolve-api-openapi.yml
  format: yaml
  label: lumify-ai Resolve API
  slug: lumify-ai-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-resolve-api-openapi.yml
- filename: lumify-ai-sports-api-openapi.yml
  format: yaml
  label: lumify-ai Sports API
  slug: lumify-ai-sports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-sports-api-openapi.yml
- filename: lumify-ai-teams-api-openapi.yml
  format: yaml
  label: lumify-ai Teams API
  slug: lumify-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-teams-api-openapi.yml
- filename: lumify-ai-trial-api-openapi.yml
  format: yaml
  label: lumify-ai Trial API
  slug: lumify-ai-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-trial-api-openapi.yml
- filename: lumify-ai-webhooks-api-openapi.yml
  format: yaml
  label: lumify-ai Webhooks API
  slug: lumify-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lumify Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: lumify-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lumify-ai
provider_slug: lumify-ai
scheme_count: 1
schemes:
- bearerFormat: lmfy-key
  description: 'Lumify API key passed as `Authorization: Bearer lmfy-...`.'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/lumify-ai-openapi.json
  type: http
slug: lumify-ai-authentication
source_filename: lumify-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/lumify-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: lmfy-key\n  description: 'Lumify API key passed as `Authorization: Bearer lmfy-...`.'\n  sources:\n  - openapi/lumify-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lumify-ai/authentication/lumify-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sports
- AI
- Real-time
- Betting
---
