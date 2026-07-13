---
api_key_in:
- header
api_specs:
- filename: appsumo-licensing-openapi.yaml
  format: yaml
  label: AppSumo Licensing API
  slug: appsumo-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsumo/refs/heads/main/openapi/appsumo-licensing-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Appsumo Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppSumo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppSumo
provider_slug: appsumo
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-AppSumo-API-Key
  sources:
  - openapi/appsumo-licensing-openapi.yaml
  type: apiKey
slug: appsumo-authentication
source_filename: appsumo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appsumo-licensing-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-AppSumo-API-Key\n  sources:\n  - openapi/appsumo-licensing-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsumo/refs/heads/main/authentication/appsumo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketplace
- SaaS
- Software Deals
---
