---
api_key_in:
- header
api_specs:
- filename: heroic-labs-nakama-openapi-original.json
  format: json
  label: Nakama API v2
  slug: nakama-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/openapi/heroic-labs-nakama-openapi-original.json
- filename: heroic-labs-nakama-console-openapi-original.json
  format: json
  label: Nakama Console API v2
  slug: nakama-console-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/openapi/heroic-labs-nakama-console-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Heroic Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heroic Labs secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heroic Labs
provider_slug: heroic-labs
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/heroic-labs-nakama-console-openapi-original.json
  - openapi/heroic-labs-nakama-openapi-original.json
  type: http
- in: header
  name: BearerJwt
  parameter: Authorization
  sources:
  - openapi/heroic-labs-nakama-console-openapi-original.json
  - openapi/heroic-labs-nakama-openapi-original.json
  type: apiKey
- in: header
  name: HttpKeyAuth
  parameter: http_key
  sources:
  - openapi/heroic-labs-nakama-openapi-original.json
  type: apiKey
slug: heroic-labs-authentication
source_filename: heroic-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/heroic-labs-nakama-console-openapi-original.json, openapi/heroic-labs-nakama-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/heroic-labs-nakama-console-openapi-original.json\n  - openapi/heroic-labs-nakama-openapi-original.json\n- name: BearerJwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/heroic-labs-nakama-console-openapi-original.json\n  - openapi/heroic-labs-nakama-openapi-original.json\n- name: HttpKeyAuth\n  type: apiKey\n  in: header\n  parameter: http_key\n  sources:\n  - openapi/heroic-labs-nakama-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/authentication/heroic-labs-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Gaming
- Game Backend
- Multiplayer
- Real-Time
- LiveOps
- Open Source
- Developer Tools
- Backend as a Service
---
