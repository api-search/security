---
api_key_in:
- header
api_specs:
- filename: thrive-global-partner-api-openapi.yml
  format: yaml
  label: Thrive Global Partner API
  slug: thrive-global-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrive-global/refs/heads/main/openapi/thrive-global-partner-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Thrive Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thrive Global secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thrive Global
provider_slug: thrive-global
scheme_count: 2
schemes:
- detail: Required only on POST /v1/auth (the token exchange).
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/thrive-global-partner-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  detail: Required on all content endpoints; 12-hour TTL.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/thrive-global-partner-api-openapi.yml
  type: http
slug: thrive-global-authentication
source_filename: thrive-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thrive-global-partner-api-openapi.yml\ndocs: https://developers.thriveglobal.com/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nflow: >-\n  Two-step: (1) POST /v1/auth with your partner API key in the x-api-key\n  header and a unique userId in the JSON body (defaults to SmokeTestUser when\n  omitted); the JWT bearer token is returned at data.logMeWith.partner.token.\n  (2) Send Authorization: Bearer <token> on every content endpoint. Tokens\n  have a 12-hour TTL - refresh proactively (e.g. after 11 hours) and handle\n  401 responses with an immediate re-auth. API keys are environment-specific\n  (staging vs production) and issued by your Thrive Global contact; there is\n  no self-serve key signup. The separate MCP server authenticates end users\n  via OAuth 2.0 / OIDC against Thrive's Keycloak IdP (client ID\n  thrive-mcp-server, roles user:mcp / user:mcp-rw).\nschemes:\n- name:\
  \ ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  detail: Required only on POST /v1/auth (the token exchange).\n  sources:\n  - openapi/thrive-global-partner-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  detail: Required on all content endpoints; 12-hour TTL.\n  sources:\n  - openapi/thrive-global-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrive-global/refs/heads/main/authentication/thrive-global-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Consumer
- Wellness
- Wellbeing
- Behavior Change
- Content
- Healthcare
- Employee Experience
---
