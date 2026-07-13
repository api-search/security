---
api_key_in:
- header
api_specs:
- filename: openapi
  format: yaml
  label: Memesio API
  slug: memesio-api
  spec_type: OpenAPI
  url: https://memesio.com/api/openapi
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Memesio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memesio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Memesio
provider_slug: memesio
scheme_count: 2
schemes:
- description: 'Optional higher-rate free-tier auth. You can also send the key as Authorization: Bearer <key>.'
  in: header
  name: DeveloperApiKeyAuth
  parameter: x-developer-api-key
  sources:
  - openapi/memesio-openapi.yml
  type: apiKey
- description: 'Agent auth for free endpoints and agent-admin routes. You can also send the key as Authorization: Bearer <key>.'
  in: header
  name: AgentApiKeyAuth
  parameter: x-agent-api-key
  sources:
  - openapi/memesio-openapi.yml
  type: apiKey
slug: memesio-authentication
source_filename: memesio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/memesio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DeveloperApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-developer-api-key\n  description: 'Optional higher-rate free-tier auth. You can also send the key as Authorization:\n    Bearer <key>.'\n  sources:\n  - openapi/memesio-openapi.yml\n- name: AgentApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-agent-api-key\n  description: 'Agent auth for free endpoints and agent-admin routes. You can also send the\n    key as Authorization: Bearer <key>.'\n  sources:\n  - openapi/memesio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/authentication/memesio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Memes
- Media
- Image Generation
- Content
- Developer Tools
---
