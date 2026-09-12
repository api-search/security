---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: publora-openapi-original.json
  format: json
  label: Publora API
  slug: publora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publora/refs/heads/main/openapi/publora-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Publora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Publora secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Publora
provider_slug: publora
scheme_count: 1
schemes:
- description: 'API key from Settings > API Keys. Format: sk_timestamp.hexstring'
  in: header
  name: ApiKeyAuth
  parameter: x-publora-key
  sources:
  - openapi/publora-openapi-original.json
  type: apiKey
slug: publora-authentication
source_filename: publora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: derived\nsource: openapi/publora-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-publora-key\n  description: 'API key from Settings > API Keys. Format: sk_timestamp.hexstring'\n  sources:\n  - openapi/publora-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publora/refs/heads/main/authentication/publora-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media
- Publishing
- Scheduling
- MCP
- Content
- Social Media Management
- Webhooks
- AI Agents
---
