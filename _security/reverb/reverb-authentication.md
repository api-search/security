---
api_key_in:
- header
api_specs:
- filename: reverb-openapi.yml
  format: yaml
  label: Reverb REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reverb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reverb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reverb
provider_slug: reverb
scheme_count: 1
schemes:
- description: 'Token returned by POST /api/auth/tokens, supplied on subsequent calls in

    the `X-Auth-Token` request header.'
  in: header
  name: XAuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/reverb-openapi.yml
  type: apiKey
slug: reverb-authentication
source_filename: reverb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reverb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: XAuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: |-\n    Token returned by POST /api/auth/tokens, supplied on subsequent calls in\n    the `X-Auth-Token` request header.\n  sources:\n  - openapi/reverb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/authentication/reverb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketplace
- Music
- Instruments
- Ecommerce
---
