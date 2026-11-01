---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: shirabe-dev-calendar-api-openapi.yml
  format: yaml
  label: shirabe-dev Calendar API
  slug: shirabe-dev-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-calendar-api-openapi.yml
- filename: shirabe-dev-hub-api-openapi.yml
  format: yaml
  label: shirabe-dev Hub API
  slug: shirabe-dev-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-hub-api-openapi.yml
- filename: shirabe-dev-system-api-openapi.yml
  format: yaml
  label: shirabe-dev System API
  slug: shirabe-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-system-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Shirabe Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: shirabe-dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: shirabe-dev
provider_slug: shirabe-dev
scheme_count: 1
schemes:
- description: APIキー（`shrb_` + 32 文字の英数字）を `X-API-Key` ヘッダーに付与する。
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/shirabe-dev-openapi.yaml
  type: apiKey
slug: shirabe-dev-authentication
source_filename: shirabe-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/shirabe-dev-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: APIキー（`shrb_` + 32 文字の英数字）を `X-API-Key` ヘッダーに付与する。\n  sources:\n  - openapi/shirabe-dev-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/shirabe-dev/authentication/shirabe-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Platform
- Japanese Data
- Deterministic
- Free Tier
- AI Integration
---
