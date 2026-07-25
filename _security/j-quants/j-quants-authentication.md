---
api_key_in:
- header
api_specs:
- filename: j-quants-derivatives-api-openapi.yml
  format: yaml
  label: J-Quants Derivatives API
  slug: j-quants-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-derivatives-api-openapi.yml
- filename: j-quants-equities-api-openapi.yml
  format: yaml
  label: J-Quants Equities API
  slug: j-quants-equities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-equities-api-openapi.yml
- filename: j-quants-fins-api-openapi.yml
  format: yaml
  label: J-Quants Fins API
  slug: j-quants-fins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-fins-api-openapi.yml
- filename: j-quants-indices-api-openapi.yml
  format: yaml
  label: J-Quants Indices API
  slug: j-quants-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-indices-api-openapi.yml
- filename: j-quants-listed-api-openapi.yml
  format: yaml
  label: J-Quants Listed API
  slug: j-quants-listed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-listed-api-openapi.yml
- filename: j-quants-markets-api-openapi.yml
  format: yaml
  label: J-Quants Markets API
  slug: j-quants-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-markets-api-openapi.yml
- filename: j-quants-option-api-openapi.yml
  format: yaml
  label: J-Quants Option API
  slug: j-quants-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-option-api-openapi.yml
- filename: j-quants-prices-api-openapi.yml
  format: yaml
  label: J-Quants Prices API
  slug: j-quants-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-prices-api-openapi.yml
- filename: j-quants-token-api-openapi.yml
  format: yaml
  label: J-Quants Token API
  slug: j-quants-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: J Quants Authentication
name_suffix: Authentication
oauth_flows: []
overview: J-Quants secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: J-Quants
provider_slug: j-quants
scheme_count: 2
schemes:
- description: Bearer ID token issued via /token/auth_refresh
  in: header
  name: idToken
  parameter: Authorization
  sources:
  - openapi/j-quants-openapi.yml
  type: apiKey
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/j-quants-openapi.yml
  type: apiKey
slug: j-quants-authentication
source_filename: j-quants-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/j-quants-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: idToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer ID token issued via /token/auth_refresh\n  sources:\n  - openapi/j-quants-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/j-quants-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/authentication/j-quants-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Financial Data
- Investment
- Japan
- Stock Market
---
