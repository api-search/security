---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: woox-account-api-openapi.yml
  format: yaml
  label: WOO X Account API
  slug: woox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-account-api-openapi.yml
- filename: woox-asset-api-openapi.yml
  format: yaml
  label: WOO X Asset API
  slug: woox-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-asset-api-openapi.yml
- filename: woox-futures-api-openapi.yml
  format: yaml
  label: WOO X Futures API
  slug: woox-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-futures-api-openapi.yml
- filename: woox-isolatedmargin-api-openapi.yml
  format: yaml
  label: WOO X Isolated Margin API
  slug: woox-isolatedmargin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-isolatedmargin-api-openapi.yml
- filename: woox-public-api-openapi.yml
  format: yaml
  label: WOO X Public API
  slug: woox-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-public-api-openapi.yml
- filename: woox-spotmargin-api-openapi.yml
  format: yaml
  label: WOO X Spot Margin API
  slug: woox-spotmargin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-spotmargin-api-openapi.yml
- filename: woox-trade-api-openapi.yml
  format: yaml
  label: WOO X Trade API
  slug: woox-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-trade-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Woox Authentication
name_suffix: Authentication
oauth_flows: []
overview: WOO X secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WOO X
provider_slug: woox
scheme_count: 5
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/woox-openapi.json
  type: http
- in: header
  name: api_key
  parameter: api_keyqq
  sources:
  - openapi/woox-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/woox-openapi.json
  type: apiKey
- in: header
  name: ApiSignAuth
  parameter: x-api-signature
  sources:
  - openapi/woox-openapi.json
  type: apiKey
- in: header
  name: ApiTimestampAuth
  parameter: x-api-timestamp
  sources:
  - openapi/woox-openapi.json
  type: apiKey
slug: woox-authentication
source_filename: woox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/woox-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/woox-openapi.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_keyqq\n  sources:\n  - openapi/woox-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/woox-openapi.json\n- name: ApiSignAuth\n  type: apiKey\n  in: header\n  parameter: x-api-signature\n  sources:\n  - openapi/woox-openapi.json\n- name: ApiTimestampAuth\n  type: apiKey\n  in: header\n  parameter: x-api-timestamp\n  sources:\n  - openapi/woox-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/authentication/woox-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Cryptocurrency
- Exchanges
- Trading
- Derivatives
---
