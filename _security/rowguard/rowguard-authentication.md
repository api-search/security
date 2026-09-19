---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rowguard-csv-validation-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog CSV validation API
  slug: rowguard-csv-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-csv-validation-api-openapi.yml
- filename: rowguard-example-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog Example API
  slug: rowguard-example-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-example-api-openapi.yml
- filename: rowguard-healthz-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog Healthz API
  slug: rowguard-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-healthz-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Rowguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: RowGuard API Catalog secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RowGuard API Catalog
provider_slug: rowguard
scheme_count: 1
schemes:
- description: Use the subscription key at the RapidAPI gateway and include X-RapidAPI-Host. The origin accepts only gateway-authenticated requests; never distribute its proxy secret.
  in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/rowguard-openapi.json
  type: apiKey
slug: rowguard-authentication
source_filename: rowguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: derived\nsource: openapi/rowguard-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: Use the subscription key at the RapidAPI gateway and include X-RapidAPI-Host.\n    The origin accepts only gateway-authenticated requests; never distribute its proxy secret.\n  sources:\n  - openapi/rowguard-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/authentication/rowguard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CSV
- Validation
- Data Quality
- Import
- Automation
---
