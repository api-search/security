---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kortexio-io-api-keys-api-openapi.yml
  format: yaml
  label: Kortexio API keys API
  slug: kortexio-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-api-keys-api-openapi.yml
- filename: kortexio-io-apps-api-openapi.yml
  format: yaml
  label: Kortexio Apps API
  slug: kortexio-io-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-apps-api-openapi.yml
- filename: kortexio-io-billing-api-openapi.yml
  format: yaml
  label: Kortexio Billing API
  slug: kortexio-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-billing-api-openapi.yml
- filename: kortexio-io-byok-api-openapi.yml
  format: yaml
  label: Kortexio BYOK API
  slug: kortexio-io-byok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-byok-api-openapi.yml
- filename: kortexio-io-mcp-api-openapi.yml
  format: yaml
  label: Kortexio MCP API
  slug: kortexio-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-mcp-api-openapi.yml
- filename: kortexio-io-memory-api-openapi.yml
  format: yaml
  label: Kortexio Memory API
  slug: kortexio-io-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-memory-api-openapi.yml
- filename: kortexio-io-meta-api-openapi.yml
  format: yaml
  label: Kortexio Meta API
  slug: kortexio-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-meta-api-openapi.yml
- filename: kortexio-io-openai-api-openapi.yml
  format: yaml
  label: Kortexio Open AI API
  slug: kortexio-io-openai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-openai-api-openapi.yml
- filename: kortexio-io-tenants-api-openapi.yml
  format: yaml
  label: Kortexio Tenants API
  slug: kortexio-io-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-tenants-api-openapi.yml
- filename: kortexio-io-chat-completions-api-openapi.yml
  format: yaml
  label: Kortexio Chat Completions API
  slug: kortexio-io-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kortexio-io/openapi/kortexio-io-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kortexio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kortexio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kortexio
provider_slug: kortexio-io
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: App API key from the dashboard (`cmk_live_...`).
  name: AppApiKey
  scheme: bearer
  sources:
  - openapi/kortexio-io-openapi.json
  type: http
slug: kortexio-io-authentication
source_filename: kortexio-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/kortexio-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AppApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: App API key from the dashboard (`cmk_live_...`).\n  sources:\n  - openapi/kortexio-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kortexio-io/authentication/kortexio-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Memory
- AI Agents
- LLM
- Europe
---
