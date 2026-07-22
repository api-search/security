---
api_key_in:
- header
api_specs:
- filename: sigma-ratings-openapi-original.json
  format: json
  label: Sigma360 API
  slug: sigma360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sigma Ratings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sigma360 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sigma360
provider_slug: sigma-ratings
scheme_count: 1
schemes:
- description: API Key
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/sigma-ratings-openapi-original.json
  type: apiKey
slug: sigma-ratings-authentication
source_filename: sigma-ratings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sigma-ratings-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key\n  sources:\n  - openapi/sigma-ratings-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/authentication/sigma-ratings-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- Financial Crime
- KYC
- AML
- Sanctions Screening
- Risk Intelligence
- RegTech
- Adverse Media
---
