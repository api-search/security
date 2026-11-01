---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: allscreenshots-com-screenshots-api-openapi.yml
  format: yaml
  label: allscreenshots-com Screenshots API
  slug: allscreenshots-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allscreenshots-com/openapi/allscreenshots-com-screenshots-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Allscreenshots Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: allscreenshots-com secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: allscreenshots-com
provider_slug: allscreenshots-com
scheme_count: 3
schemes:
- description: OAuth or dashboard access token, not a raw API key; pair with X-API-Key-Id.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/allscreenshots.json
  type: http
- description: Pass your raw API key in X-API-Key.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/allscreenshots.json
  type: apiKey
- description: Required alongside an OAuth/dashboard Bearer token; use the organization API key ID.
  in: header
  name: apiKeyId
  parameter: X-API-Key-Id
  sources:
  - openapi/allscreenshots.json
  type: apiKey
slug: allscreenshots-com-authentication
source_filename: allscreenshots-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/allscreenshots.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth or dashboard access token, not a raw API key; pair with X-API-Key-Id.\n  sources:\n  - openapi/allscreenshots.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Pass your raw API key in X-API-Key.\n  sources:\n  - openapi/allscreenshots.json\n- name: apiKeyId\n  type: apiKey\n  in: header\n  parameter: X-API-Key-Id\n  description: Required alongside an OAuth/dashboard Bearer token; use the organization API\n    key ID.\n  sources:\n  - openapi/allscreenshots.json\n"
source_yaml_url: https://artifacts.apis.io/allscreenshots-com/authentication/allscreenshots-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- ScreenshotAPI
- Automation
- Marketing
- Developers
---
