---
api_key_in:
- header
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Refinitiv Data Platform APIs
  slug: refinitiv-data-platform-apis
  spec_type: OpenAPI
  url: https://api.refinitiv.com/streaming-pricing/docs/swagger.yaml
- filename: refinitiv-eikon-asyncapi.yml
  format: yaml
  label: LSEG WebSocket API
  slug: lseg-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/asyncapi/refinitiv-eikon-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Refinitiv Eikon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refinitiv Eikon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Refinitiv Eikon
provider_slug: refinitiv-eikon
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from the authentication endpoint. Access tokens are valid for five minutes and must be refreshed using the refresh token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/refinitiv-eikon-data-platform-openapi.yml
  type: http
- description: Session token obtained from the RequestToken endpoint. Include as Token followed by the token value.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/refinitiv-eikon-datascope-select-openapi.yml
  - openapi/refinitiv-eikon-tick-history-openapi.yml
  type: apiKey
slug: refinitiv-eikon-authentication
source_filename: refinitiv-eikon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/refinitiv-eikon-data-platform-openapi.yml, openapi/refinitiv-eikon-datascope-select-openapi.yml,\n  openapi/refinitiv-eikon-tick-history-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from the authentication endpoint. Access tokens\n    are valid for five minutes and must be refreshed using the refresh token.\n  sources:\n  - openapi/refinitiv-eikon-data-platform-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Session token obtained from the RequestToken endpoint. Include as Token followed\n    by the token value.\n  sources:\n  - openapi/refinitiv-eikon-datascope-select-openapi.yml\n  - openapi/refinitiv-eikon-tick-history-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/authentication/refinitiv-eikon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Financial Data
- Financial News
- Market Data
- Real-Time Data
- Trading
---
