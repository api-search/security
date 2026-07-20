---
api_key_in:
- header
api_specs:
- filename: got-its-openapi-original.yml
  format: yaml
  label: Reelables API
  slug: reelables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-openapi-original.yml
- filename: got-its-gateway-openapi-original.yml
  format: yaml
  label: Reelables Gateway API
  slug: reelables-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-gateway-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Got Its Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Reelables secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Reelables
provider_slug: got-its
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/got-its-gateway-openapi-original.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.reelables.com/oauth2/token
  name: AuthEndpoint
  sources:
  - openapi/got-its-openapi-original.yml
  type: oauth2
slug: got-its-authentication
source_filename: got-its-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/got-its-gateway-openapi-original.yml, openapi/got-its-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/got-its-gateway-openapi-original.yml\n- name: AuthEndpoint\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.reelables.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/got-its-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/authentication/got-its-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Supply Chain
- Logistics
- Asset Tracking
- IoT
- Smart Labels
- Bluetooth
- Cellular
- Track and Trace
- Location
---
