---
api_key_in:
- header
api_specs:
- filename: goodhire-packages-api-openapi.yml
  format: yaml
  label: GoodHire Packages API
  slug: goodhire-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-packages-api-openapi.yml
- filename: goodhire-partner-api-openapi.yml
  format: yaml
  label: GoodHire Partner API
  slug: goodhire-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-partner-api-openapi.yml
- filename: goodhire-reports-api-openapi.yml
  format: yaml
  label: GoodHire Reports API
  slug: goodhire-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-reports-api-openapi.yml
- filename: goodhire-requestors-api-openapi.yml
  format: yaml
  label: GoodHire Requestors API
  slug: goodhire-requestors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-requestors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Goodhire Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoodHire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoodHire
provider_slug: goodhire
scheme_count: 1
schemes:
- description: 'API key sent as: Authorization: ApiKey <API_KEY>. Request keys from api@goodhire.com.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/goodhire-openapi.yml
  type: apiKey
slug: goodhire-authentication
source_filename: goodhire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goodhire-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key sent as: Authorization: ApiKey <API_KEY>. Request keys from api@goodhire.com.'\n  sources:\n  - openapi/goodhire-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/authentication/goodhire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Background Checks
- Employment Screening
- Identity Verification
- HR
- Compliance
- FCRA
- Checkr
---
