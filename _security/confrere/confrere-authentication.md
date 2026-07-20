---
api_key_in:
- header
api_specs:
- filename: confrere-video-openapi.yml
  format: yaml
  label: Confrere Video API
  slug: confrere-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/openapi/confrere-video-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Confrere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confrere secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Confrere
provider_slug: confrere
scheme_count: 3
schemes:
- description: 'Signed bearer token for the request, sent as `Authorization: Bearer $TOKEN`. Paired with the X-Vidicue-Nonce and X-Vidicue-Key headers.'
  format: Bearer $TOKEN
  header: Authorization
  in: header
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/confrere-video-openapi.yml
  type: http
- description: The API key issued for your integration.
  header: X-Vidicue-Key
  in: header
  name: ApiKey
  sources:
  - openapi/confrere-video-openapi.yml
  type: apiKey
- description: A numeric nonce accompanying the bearer authorization.
  header: X-Vidicue-Nonce
  in: header
  name: Nonce
  sources:
  - openapi/confrere-video-openapi.yml
  type: apiKey
slug: confrere-authentication
source_filename: confrere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.compodium.com/api/\ndocs: https://docs.compodium.com/api/\nnotes: >-\n  The published OpenAPI declares no named securitySchemes — authentication is\n  documented as three required request headers on every operation. Captured\n  here from the docs rather than derived from an (absent) securitySchemes block.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Bearer $TOKEN\"\n    description: >-\n      Signed bearer token for the request, sent as `Authorization: Bearer\n      $TOKEN`. Paired with the X-Vidicue-Nonce and X-Vidicue-Key headers.\n    sources: [openapi/confrere-video-openapi.yml]\n  - name: ApiKey\n    type: apiKey\n    in: header\n    header: X-Vidicue-Key\n    description: The API key issued for your integration.\n    sources: [openapi/confrere-video-openapi.yml]\n\
  \  - name: Nonce\n    type: apiKey\n    in: header\n    header: X-Vidicue-Nonce\n    description: A numeric nonce accompanying the bearer authorization.\n    sources: [openapi/confrere-video-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/authentication/confrere-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Video
- Video Conferencing
- Communications
- Healthcare
- Telehealth
- Embeddable
- WebRTC
---
