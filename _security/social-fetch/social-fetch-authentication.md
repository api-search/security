---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Social Fetch REST API
  slug: social-fetch-rest-api
  spec_type: OpenAPI
  url: https://www.socialfetch.dev/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Social Fetch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Social Fetch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Social Fetch
provider_slug: social-fetch
scheme_count: 1
schemes:
- description: API key (`sfk_...`)
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/social-fetch-openapi.json
  type: apiKey
slug: social-fetch-authentication
source_filename: social-fetch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: derived\nsource: openapi/social-fetch-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key (`sfk_...`)\n  sources:\n  - openapi/social-fetch-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/social-fetch/refs/heads/main/authentication/social-fetch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- social media
- web scraping
- data extraction
- social listening
- monitoring
- structured data
- JSON API
- REST
- MCP
- agent-native
- TypeScript SDK
- transcripts
- ads intelligence
---
