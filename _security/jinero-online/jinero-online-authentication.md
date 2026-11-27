---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Jinero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jinero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jinero
provider_slug: jinero-online
scheme_count: 1
schemes:
- description: Optional. Personal API token from your dashboard — identifies you for bookmarks and user endpoints (it does not raise the rate limit). Bearer header is also accepted.
  in: header
  name: ApiToken
  parameter: X-API-Token
  sources:
  - openapi/jinero-online-openapi.json
  type: apiKey
slug: jinero-online-authentication
source_filename: jinero-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/jinero-online-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  description: Optional. Personal API token from your dashboard — identifies you for bookmarks\n    and user endpoints (it does not raise the rate limit). Bearer header is also accepted.\n  sources:\n  - openapi/jinero-online-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/jinero-online/authentication/jinero-online-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Design Tools
- Free
- Web
- Figma
- Image Processing
---
