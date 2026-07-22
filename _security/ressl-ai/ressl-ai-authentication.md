---
api_key_in:
- header
api_specs:
- filename: ressl-ai-platform-openapi.yml
  format: yaml
  label: Ressl Platform API
  slug: ressl-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ressl-ai/refs/heads/main/openapi/ressl-ai-platform-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ressl Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ressl secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ressl
provider_slug: ressl-ai
scheme_count: 2
schemes:
- description: Organization API key (prefix rsk_) sent as a bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ressl-ai-platform-openapi.yml
  type: http
- description: Organization API key (prefix rsk_) sent in the X-API-Key header.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/ressl-ai-platform-openapi.yml
  type: apiKey
slug: ressl-ai-authentication
source_filename: ressl-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ressl-ai-platform-openapi.yml\ndocs: https://docs.ressl.ai/api-reference/authentication\nnotes: >-\n  Control-plane requests use an organization API key (prefix rsk_) created in\n  the simulation.ressl.ai console (Settings, API keys), sent either as\n  Authorization: Bearer rsk_... or X-API-Key: rsk_.... Keys are org-scoped and\n  shown once at creation. Missing, malformed, or revoked keys return 401\n  { \"error\": \"Unauthorized\" }. The human console itself authenticates via\n  WorkOS AuthKit; the rsk_ key is the programmatic credential.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization API key (prefix rsk_) sent as a bearer token.\n  sources:\n  - openapi/ressl-ai-platform-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organization API key (prefix rsk_)\
  \ sent in the X-API-Key header.\n  sources:\n  - openapi/ressl-ai-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ressl-ai/refs/heads/main/authentication/ressl-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Mock APIs
- API Testing
- AI Agents
- Agent Evaluation
- Sandbox
- Developer Tools
- Synthetic Data
- SaaS
---
