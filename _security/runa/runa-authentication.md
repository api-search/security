---
api_key_in:
- header
api_specs:
- filename: runa-payouts-api-openapi.yml
  format: yaml
  label: Runa Payouts API
  slug: runa-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runa/refs/heads/main/openapi/runa-payouts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Runa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runa
provider_slug: runa
scheme_count: 1
schemes:
- description: Runa API key. Generate your key at https://app.runa.io/api-keys. The key is only displayed at generation time for security.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/runa-payouts-api-openapi.yml
  type: apiKey
slug: runa-authentication
source_filename: runa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runa-payouts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Runa API key. Generate your key at https://app.runa.io/api-keys. The key is only\n    displayed at generation time for security.\n  sources:\n  - openapi/runa-payouts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runa/refs/heads/main/authentication/runa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Gift Cards
- Rewards
- Payments
- Incentives
- Payouts
---
