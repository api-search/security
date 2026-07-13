---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Hex.pm API
  slug: hexpm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hex Pm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hex.pm secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hex.pm
provider_slug: hex-pm
scheme_count: 3
schemes:
- description: 'API token authentication. Pass the token directly: `Authorization: token`. For OAuth2 Bearer tokens use: `Authorization: Bearer token`.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
- description: OAuth2 Bearer token obtained via Device Authorization Grant (RFC 8628).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
- description: Deprecated. Basic authentication with username and password. Only allowed on specific endpoints for generating API tokens.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
slug: hex-pm-authentication
source_filename: hex-pm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token authentication. Pass the token directly: `Authorization: token`. For\n    OAuth2 Bearer tokens use: `Authorization: Bearer token`.'\n  sources:\n  - openapi/openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer token obtained via Device Authorization Grant (RFC 8628).\n  sources:\n  - openapi/openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Deprecated. Basic authentication with username and password. Only allowed on\n    specific endpoints for generating API tokens.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/authentication/hex-pm-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Package Registry
- Erlang
- Elixir
- Gleam
- BEAM
- Open Source
- Package Manager
---
