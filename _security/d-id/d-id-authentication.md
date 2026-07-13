---
api_key_in:
- header
api_specs:
- filename: d-id-videos-openapi.yml
  format: yaml
  label: D-ID Videos API
  slug: d-id-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/openapi/d-id-videos-openapi.yml
- filename: d-id-agents-openapi.yml
  format: yaml
  label: D-ID Agents API
  slug: d-id-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/openapi/d-id-agents-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: D Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: D-ID secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: D-ID
provider_slug: d-id
scheme_count: 3
schemes:
- description: HTTP Basic Authentication using API key as username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/d-id-agents-openapi.yml
  - openapi/d-id-videos-openapi.yml
  type: http
- description: Bearer token authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/d-id-agents-openapi.yml
  - openapi/d-id-videos-openapi.yml
  type: http
- description: Scoped client key for SDK embedding.
  in: header
  name: clientKeyAuth
  parameter: Authorization
  sources:
  - openapi/d-id-agents-openapi.yml
  type: apiKey
slug: d-id-authentication
source_filename: d-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/d-id-agents-openapi.yml, openapi/d-id-videos-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using API key as username.\n  sources:\n  - openapi/d-id-agents-openapi.yml\n  - openapi/d-id-videos-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication.\n  sources:\n  - openapi/d-id-agents-openapi.yml\n  - openapi/d-id-videos-openapi.yml\n- name: clientKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Scoped client key for SDK embedding.\n  sources:\n  - openapi/d-id-agents-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/authentication/d-id-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI Video
- Digital Humans
- Talking Head
- Avatar
- Generative AI
- Video Generation
- Real-Time Streaming
- Text to Video
- Video Translation
- Voice Cloning
---
