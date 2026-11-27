---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chirpie-ai-openapi-generated.yml
  format: yaml
  label: Chirpie API
  slug: chirpie-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chirpie-ai/openapi/_ae-authored/chirpie-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chirpie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chirpie declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chirpie
provider_slug: chirpie-ai
scheme_count: 2
schemes:
- applies_to: REST API https://chirpie.ai/api/v1
  detail: API keys are prefixed with chirpie_sk_ followed by a 40-character random string, hashed with SHA-256 before storage. Up to 25 active keys per account; each key expires 90 days after creation; revoked keys stop working immediately. Keys can be narrowed with scopes (null = full access).
  format: Bearer chirpie_sk_<40 chars>
  header: Authorization
  in: header
  key_prefix: chirpie_sk_
  name: apiKey
  scheme: bearer
  type: http
- applies_to: Hosted MCP server https://chirpie.ai/mcp
  detail: Per the MCP docs, the client walks the user through Chirpie sign-in the first time ("signs you in with OAuth"); no API key to paste. The endpoint answered 401 unauthenticated in pre-flight.
  docs: https://chirpie.ai/docs/mcp
  name: mcpOAuth
  type: oauth2
slug: chirpie-ai-authentication
source_filename: chirpie-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chirpie.ai/docs/authentication.md\ndocs: https://chirpie.ai/docs/authentication\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer chirpie_sk_<40 chars>\n  key_prefix: chirpie_sk_\n  applies_to: REST API https://chirpie.ai/api/v1\n  detail: API keys are prefixed with chirpie_sk_ followed by a 40-character random string, hashed with SHA-256 before\n    storage. Up to 25 active keys per account; each key expires 90 days after creation; revoked keys stop working\n    immediately. Keys can be narrowed with scopes (null = full access).\n- name: mcpOAuth\n  type: oauth2\n  applies_to: Hosted MCP server https://chirpie.ai/mcp\n  detail: Per the MCP docs, the client walks the user through Chirpie sign-in the first time (\"signs you in with\n    OAuth\"); no API key to paste. The endpoint answered 401 unauthenticated in pre-flight.\n  docs: https://chirpie.ai/docs/mcp\n\
  key_management:\n  create: POST /api/v1/keys\n  list: GET /api/v1/keys\n  revoke: DELETE /api/v1/keys?id=KEY_ID\n  max_active_keys: 25\n  expiry: 90 days\nnote: The AE-generated OpenAPI declares no securitySchemes, so derive-authentication.py produced nothing; this profile\n  is read from the docs.\n"
source_yaml_url: https://artifacts.apis.io/chirpie-ai/authentication/chirpie-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Social Media
- Social Media Posting
- Scheduling
- MCP
- AI Agents
- Analytics
---
