---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Imaginode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imaginode declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Imaginode
provider_slug: imaginode
scheme_count: 1
schemes:
- description: Account API key sent as a bearer token. Keys are created in the user profile under "API keys" (requires a verified email); the imk_ secret is shown only once at creation. At most 5 active keys per account; a key is revocable at any time and stops working immediately. Each key is limited to 10 generations per minute.
  header: 'Authorization: Bearer imk_...'
  id: api-key-bearer
  key_prefix: imk_
  scheme: bearer
  surfaces:
  - REST API (POST /api/generate, GET /api/generate/status)
  - MCP server (https://imaginode.ai/api/mcp, tool calls)
  type: http
slug: imaginode-authentication
source_filename: imaginode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://imaginode.ai/en/docs/api-mcp\ndocs: https://imaginode.ai/en/docs/api-mcp\nnote: >-\n  No OpenAPI is published; this profile is read from the provider's API & MCP documentation\n  and confirmed by live unauthenticated probes (POST /api/generate and\n  GET /api/generate/status both return 401 {\"error\": \"Non authentifie\"} without a key;\n  GET /api/models and MCP tools/list answer anonymously).\nschemes:\n  - id: api-key-bearer\n    type: http\n    scheme: bearer\n    key_prefix: imk_\n    header: 'Authorization: Bearer imk_...'\n    surfaces:\n      - REST API (POST /api/generate, GET /api/generate/status)\n      - MCP server (https://imaginode.ai/api/mcp, tool calls)\n    description: >-\n      Account API key sent as a bearer token. Keys are created in the user profile under\n      \"API keys\" (requires a verified email); the imk_ secret is shown only once at creation.\n      At most 5 active keys per account;\
  \ a key is revocable at any time and stops working\n      immediately. Each key is limited to 10 generations per minute.\nunauthenticated_surfaces:\n  - GET /api/models (model catalog and per-model credit pricing)\n  - MCP tools/list (tool discovery with full inputSchemas)\noauth: none documented\nkey_management:\n  create: user profile, section \"API keys\" (verified email required)\n  max_active_keys: 5\n  revocation: one click from the profile; immediate\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imaginode/refs/heads/main/authentication/imaginode-authentication.yml
summary_line: 1 scheme
tags:
- ai
- image generation
- video generation
- text to speech
- mcp
- generative ai
- llm
- creative tools
---
