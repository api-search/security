---
api_key_in: []
api_specs:
- filename: exchangerate-openapi.yml
  format: yaml
  label: ExchangeRate-API
  slug: exchangerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate/refs/heads/main/openapi/exchangerate-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Exchangerate Authentication
name_suffix: Authentication
oauth_flows: []
overview: ExchangeRate-API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ExchangeRate-API
provider_slug: exchangerate
scheme_count: 1
schemes:
- description: 'Pass API key as a Bearer token in the Authorization header (e.g. Authorization: Bearer YOUR-API-KEY). When using this method, omit the API key from the URL path. The path-key endpoints do not use a security scheme in the OpenAPI sense; the {apiKey} path parameter serves as the credential.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/exchangerate-openapi.yml
  type: http
slug: exchangerate-authentication
source_filename: exchangerate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exchangerate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass API key as a Bearer token in the Authorization header (e.g. Authorization:\n    Bearer YOUR-API-KEY). When using this method, omit the API key from the URL path. The path-key\n    endpoints do not use a security scheme in the OpenAPI sense; the {apiKey} path parameter\n    serves as the credential.'\n  sources:\n  - openapi/exchangerate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate/refs/heads/main/authentication/exchangerate-authentication.yml
summary_line: http · 1 scheme
tags:
- Currency
- Exchange Rates
- Finance
- Forex
- Financial Data
- Currency Conversion
---
