---
api_key_in:
- header
api_specs:
- filename: uniform-platform-api-openapi.json
  format: json
  label: Uniform Platform API
  slug: uniform-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniform/refs/heads/main/openapi/uniform-platform-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uniform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uniform secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uniform
provider_slug: uniform
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/uniform-platform-api-openapi.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/uniform-platform-api-openapi.json
  type: http
slug: uniform-authentication
source_filename: uniform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/uniform-platform-api-openapi.json\ndocs: https://docs.uniform.app/docs/guides/api-access\nnotes: >-\n  Two credential types back the two schemes: service accounts (machine\n  identities with assigned roles, formerly \"API keys\"; recommended for\n  integrations, CI/CD, and server-side use, optional expiration, survive\n  personnel changes) and personal access tokens (tied to a user, capped to\n  the owner's current roles, max 10 per user per team; recommended for the\n  MCP server, Chrome extension, and local development). Keys are sent in the\n  x-api-key header (ApiKeyAuth) or as a bearer token (BearerAuth). Credential\n  operations are recorded in a 30-day security audit log. Environment\n  variables UNIFORM_API_KEY / UNIFORM_CLI_API_KEY are used by the SDKs/CLI.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n\
  \  sources:\n  - openapi/uniform-platform-api-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/uniform-platform-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniform/refs/heads/main/authentication/uniform-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Digital Experience Platform
- Content Management
- Personalization
- AB Testing
- Composable
- Headless CMS
- AI Agents
- Webhooks
---
