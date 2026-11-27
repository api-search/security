---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nimcoffee-com-default-api-openapi.yml
  format: yaml
  label: NiM Coffee 产品 API
  slug: nimcoffee-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimcoffee-com/openapi/nimcoffee-com-default-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NiM Coffee Authentication
name_suffix: Authentication
oauth_flows: []
overview: NiM Coffee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NiM Coffee
provider_slug: nimcoffee-com
scheme_count: 1
schemes:
- description: API 密钥。在 https://nimcoffee.com/open 自助签发，提交即刻生效。
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nimcoffee-com-openapi.json
  type: apiKey
slug: nimcoffee-com-authentication
source_filename: nimcoffee-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nimcoffee-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API 密钥。在 https://nimcoffee.com/open 自助签发，提交即刻生效。\n  sources:\n  - openapi/nimcoffee-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nimcoffee-com/authentication/nimcoffee-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Coffee
- AI Platform
---
