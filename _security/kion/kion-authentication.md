---
api_key_in: []
api_specs:
- filename: kion-cloud-operations-api-openapi.yml
  format: yaml
  label: Kion Cloud Operations API
  slug: kion-cloud-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/openapi/kion-cloud-operations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kion
provider_slug: kion
scheme_count: 1
schemes:
- description: 'Kion App API Key. Generate in Kion under your user profile settings. Use in the Authorization header as: Bearer [example key]'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kion-cloud-operations-api-openapi.yml
  type: http
slug: kion-authentication
source_filename: kion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kion-cloud-operations-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Kion App API Key. Generate in Kion under your user profile settings. Use in\n    the Authorization header as: Bearer [example key]'\n  sources:\n  - openapi/kion-cloud-operations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/authentication/kion-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
---
