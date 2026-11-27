---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clipia-ai-account-api-openapi.yml
  format: yaml
  label: Clipia.ai Account API
  slug: clipia-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-account-api-openapi.yml
- filename: clipia-ai-llm-api-openapi.yml
  format: yaml
  label: Clipia.ai LLM API
  slug: clipia-ai-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-llm-api-openapi.yml
- filename: clipia-ai-models-api-openapi.yml
  format: yaml
  label: Clipia.ai Models API
  slug: clipia-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-models-api-openapi.yml
- filename: clipia-ai-queue-api-openapi.yml
  format: yaml
  label: Clipia.ai Queue API
  slug: clipia-ai-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-queue-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clipia.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clipia.ai secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clipia.ai
provider_slug: clipia-ai
scheme_count: 2
schemes:
- description: 'API key sent as `Authorization: Bearer clipia_live_…` (recommended; accepts only keys starting with `clipia_`). The server also accepts `Authorization: Key <key>` (case-insensitive) and the `X-Api-Key: <key>` header.'
  header_forms:
  - 'Authorization: Bearer …'
  - 'Authorization: Key …'
  - 'X-Api-Key: …'
  in: header
  key_prefixes:
    live: clipia_live_
    test: clipia_test_
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/clipia-ai-openapi.yml
  - https://clipia.ai/en/docs/getting-started/authentication
  type: apiKey
- applies_to: https://mcp.clipia.ai/mcp
  description: 'MCP server only: "Sign in with a Clipia API key or with your Clipia account over OAuth." claude.ai connects via sign-in to the Clipia account (OAuth); no key required.'
  name: mcp-oauth
  sources:
  - https://clipia.ai/en/docs/mcp
  type: oauth2
slug: clipia-ai-authentication
source_filename: clipia-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clipia.ai/en/docs/getting-started/authentication\ndocs: https://clipia.ai/en/docs/getting-started/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key sent as `Authorization: Bearer clipia_live_…` (recommended; accepts only keys starting with `clipia_`). The server also accepts `Authorization: Key <key>` (case-insensitive) and the `X-Api-Key: <key>` header.'\n  header_forms:\n  - 'Authorization: Bearer …'\n  - 'Authorization: Key …'\n  - 'X-Api-Key: …'\n  key_prefixes:\n    live: clipia_live_\n    test: clipia_test_\n  sources:\n  - openapi/clipia-ai-openapi.yml\n  - https://clipia.ai/en/docs/getting-started/authentication\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://mcp.clipia.ai/mcp\n  description: 'MCP server only: \"Sign in with a Clipia API key or with your Clipia account\
  \ over OAuth.\" claude.ai connects via sign-in to the Clipia account (OAuth); no key required.'\n  sources:\n  - https://clipia.ai/en/docs/mcp\nkey_management:\n  console: https://clipia.ai/en/developer\n  shown_once: true\n  max_active_keys: 20\n  limit_error: 400 api_key_limit_reached\n  live_key_requirement: Generation with a clipia_live_ key is available to accounts that have bought credits at least once; otherwise 402 insufficient_credits.\n"
source_yaml_url: https://artifacts.apis.io/clipia-ai/authentication/clipia-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Video Generation
- Image Generation
- Generative AI
- MCP
---
