---
api_key_in:
- header
api_specs:
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Sandbox API
  slug: e2b-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Template API
  slug: e2b-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Volume API
  slug: e2b-volume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-events-openapi.yml
  format: yaml
  label: E2B Sandbox Events and Webhooks API
  slug: e2b-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-events-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Team and Identity API
  slug: e2b-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: E2B Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: E2B secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: E2B
provider_slug: e2b-dev
scheme_count: 5
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/e2b-api-openapi.yml
  - openapi/e2b-events-openapi.yml
  type: apiKey
- bearerFormat: access_token
  name: AccessTokenAuth
  scheme: bearer
  sources:
  - openapi/e2b-api-openapi.yml
  - openapi/e2b-volumes-openapi.yml
  type: http
- in: header
  name: Supabase1TokenAuth
  parameter: X-Supabase-Token
  sources:
  - openapi/e2b-api-openapi.yml
  type: apiKey
- in: header
  name: Supabase2TeamAuth
  parameter: X-Supabase-Team
  sources:
  - openapi/e2b-api-openapi.yml
  type: apiKey
- in: header
  name: AdminTokenAuth
  parameter: X-Admin-Token
  sources:
  - openapi/e2b-api-openapi.yml
  type: apiKey
slug: e2b-dev-authentication
source_filename: e2b-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/e2b-api-openapi.yml, openapi/e2b-events-openapi.yml, openapi/e2b-volumes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/e2b-api-openapi.yml\n  - openapi/e2b-events-openapi.yml\n- name: AccessTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  sources:\n  - openapi/e2b-api-openapi.yml\n  - openapi/e2b-volumes-openapi.yml\n- name: Supabase1TokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Supabase-Token\n  sources:\n  - openapi/e2b-api-openapi.yml\n- name: Supabase2TeamAuth\n  type: apiKey\n  in: header\n  parameter: X-Supabase-Team\n  sources:\n  - openapi/e2b-api-openapi.yml\n- name: AdminTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Admin-Token\n  sources:\n  - openapi/e2b-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/authentication/e2b-dev-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- AI
- Agents
- Code Execution
- Code Interpreter
- Sandboxes
- Firecracker
- microVMs
- Computer Use
- Desktop Sandbox
- Templates
- MCP
- Open Source
---
