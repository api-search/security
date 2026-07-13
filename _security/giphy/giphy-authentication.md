---
api_key_in:
- query
api_specs:
- filename: giphy-openapi.yml
  format: yaml
  label: GIPHY API
  slug: giphy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Giphy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giphy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Giphy
provider_slug: giphy
scheme_count: 1
schemes:
- description: API key issued via the GIPHY developer dashboard.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/giphy-openapi.yml
  type: apiKey
slug: giphy-authentication
source_filename: giphy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/giphy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key issued via the GIPHY developer dashboard.\n  sources:\n  - openapi/giphy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/authentication/giphy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Photography
- Media
- GIFs
- Stickers
- Emoji
- Video
- Messaging
- Social
- Meta
---
