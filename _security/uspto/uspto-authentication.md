---
api_key_in:
- header
api_specs:
- filename: uspto-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-assignments-api-openapi.yml
- filename: uspto-patents-api-openapi.yml
  format: yaml
  label: USPTO Patents API
  slug: uspto-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-patents-api-openapi.yml
- filename: uspto-ptab-api-openapi.yml
  format: yaml
  label: USPTO PTAB API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-ptab-api-openapi.yml
- filename: uspto-trademarks-api-openapi.yml
  format: yaml
  label: USPTO Trademarks API
  slug: uspto-trademarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-trademarks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uspto Authentication
name_suffix: Authentication
oauth_flows: []
overview: USPTO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: USPTO
provider_slug: uspto
scheme_count: 1
schemes:
- description: USPTO Open Data Portal API key
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/uspto-patent-api-openapi.yml
  type: apiKey
slug: uspto-authentication
source_filename: uspto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uspto-patent-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: USPTO Open Data Portal API key\n  sources:\n  - openapi/uspto-patent-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/authentication/uspto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Intellectual Property
- Open Data
- Patents
- Regulatory
- Trademarks
- USPTO
---
