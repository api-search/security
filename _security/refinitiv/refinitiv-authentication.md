---
api_key_in:
- header
api_specs:
- filename: refinitiv-data-platform-openapi.yml
  format: yaml
  label: Refinitiv Data Platform (RDP) API
  slug: refinitiv-data-platform-rdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-data-platform-openapi.yml
- filename: refinitiv-real-time-websocket-asyncapi.yml
  format: yaml
  label: Refinitiv Real-Time WebSocket API
  slug: refinitiv-real-time-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/asyncapi/refinitiv-real-time-websocket-asyncapi.yml
- filename: refinitiv-datascope-select-openapi.yml
  format: yaml
  label: LSEG DataScope Select - REST API
  slug: lseg-datascope-select-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-datascope-select-openapi.yml
- filename: refinitiv-world-check-one-openapi.yml
  format: yaml
  label: World-Check One API
  slug: world-check-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-world-check-one-openapi.yml
- filename: refinitiv-qual-id-openapi.yml
  format: yaml
  label: Qual-ID API
  slug: qual-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-qual-id-openapi.yml
- filename: refinitiv-permid-entity-search-openapi.yml
  format: yaml
  label: PermID Entity Search API
  slug: permid-entity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-permid-entity-search-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Refinitiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refinitiv secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Refinitiv
provider_slug: refinitiv
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from the /auth/oauth2/v1/token endpoint. Access tokens are valid for five minutes.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/refinitiv-data-platform-openapi.yml
  type: http
- description: Session token obtained from the Authentication/RequestToken endpoint. Include as Token followed by the token value.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/refinitiv-datascope-select-openapi.yml
  - openapi/refinitiv-world-check-one-openapi.yml
  type: apiKey
- description: Open PermID API key. Registered users receive an API key that is shared across PermID Entity Search, Record Matching, and Intelligent Tagging services.
  in: header
  name: apiKeyAuth
  parameter: x-ag-access-token
  sources:
  - openapi/refinitiv-permid-entity-search-openapi.yml
  type: apiKey
- description: HTTP Basic Authentication using Base64-encoded username and password credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/refinitiv-qual-id-openapi.yml
  type: http
slug: refinitiv-authentication
source_filename: refinitiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/refinitiv-data-platform-openapi.yml, openapi/refinitiv-datascope-select-openapi.yml,\n  openapi/refinitiv-permid-entity-search-openapi.yml, openapi/refinitiv-qual-id-openapi.yml,\n  openapi/refinitiv-world-check-one-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from the /auth/oauth2/v1/token endpoint. Access\n    tokens are valid for five minutes.\n  sources:\n  - openapi/refinitiv-data-platform-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Session token obtained from the Authentication/RequestToken endpoint. Include\n    as Token followed by the token value.\n  sources:\n  - openapi/refinitiv-datascope-select-openapi.yml\n  - openapi/refinitiv-world-check-one-openapi.yml\n- name: apiKeyAuth\n  type:\
  \ apiKey\n  in: header\n  parameter: x-ag-access-token\n  description: Open PermID API key. Registered users receive an API key that is shared across\n    PermID Entity Search, Record Matching, and Intelligent Tagging services.\n  sources:\n  - openapi/refinitiv-permid-entity-search-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Base64-encoded username and password credentials.\n  sources:\n  - openapi/refinitiv-qual-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/authentication/refinitiv-authentication.yml
summary_line: apiKey/http · 4 schemes
tags: []
---
