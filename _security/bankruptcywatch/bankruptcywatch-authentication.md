---
api_key_in:
- header
api_specs:
- filename: bankruptcywatch-pacer-api-openapi.yml
  format: yaml
  label: BankruptcyWatch PACER API
  slug: pacer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/openapi/bankruptcywatch-pacer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bankruptcywatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: BankruptcyWatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
scheme_count: 1
schemes:
- description: BankruptcyWatch API key
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/bankruptcywatch-pacer-api-openapi.yml
  type: apiKey
slug: bankruptcywatch-authentication
source_filename: bankruptcywatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bankruptcywatch-pacer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: BankruptcyWatch API key\n  sources:\n  - openapi/bankruptcywatch-pacer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/authentication/bankruptcywatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
---
