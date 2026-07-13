---
api_key_in:
- header
api_specs:
- filename: taddy-podcast-openapi.yml
  format: yaml
  label: Taddy Podcast API
  slug: taddy-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taddy-api/refs/heads/main/openapi/taddy-podcast-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Taddy Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taddy API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Taddy API
provider_slug: taddy-api
scheme_count: 2
schemes:
- description: Your Taddy API key from the developer dashboard
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/taddy-podcast-openapi.yml
  type: apiKey
- description: Your Taddy user ID from the developer dashboard
  in: header
  name: UserIdAuth
  parameter: X-USER-ID
  sources:
  - openapi/taddy-podcast-openapi.yml
  type: apiKey
slug: taddy-api-authentication
source_filename: taddy-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taddy-podcast-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Your Taddy API key from the developer dashboard\n  sources:\n  - openapi/taddy-podcast-openapi.yml\n- name: UserIdAuth\n  type: apiKey\n  in: header\n  parameter: X-USER-ID\n  description: Your Taddy user ID from the developer dashboard\n  sources:\n  - openapi/taddy-podcast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taddy-api/refs/heads/main/authentication/taddy-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Audio
- Comics
- GraphQL
- Media
- Podcasts
- Transcripts
- Webhooks
---
