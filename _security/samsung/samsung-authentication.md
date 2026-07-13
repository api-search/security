---
api_key_in: []
api_specs:
- filename: samsung-smartthings-openapi.yml
  format: yaml
  label: SmartThings API
  slug: smartthings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samsung/refs/heads/main/openapi/samsung-smartthings-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Samsung Authentication
name_suffix: Authentication
oauth_flows: []
overview: Samsung secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Samsung
provider_slug: samsung
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token or SmartThings personal access token. Obtain tokens at https://account.smartthings.com/tokens.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/samsung-smartthings-openapi.yml
  type: http
slug: samsung-authentication
source_filename: samsung-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/samsung-smartthings-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token or SmartThings personal access token. Obtain tokens at\n    https://account.smartthings.com/tokens.\n  sources:\n  - openapi/samsung-smartthings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samsung/refs/heads/main/authentication/samsung-authentication.yml
summary_line: http · 1 scheme
tags:
- Consumer Electronics
- Developer Platform
- IoT
- Mobile
- Smart Home
- Smart TV
- Wearables
---
