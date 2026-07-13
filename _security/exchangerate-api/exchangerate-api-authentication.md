---
api_key_in:
- path
api_specs:
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Latest Rates API
  slug: latest-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Pair Conversion API
  slug: pair-conversion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Enriched Data API
  slug: enriched-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Historical Rates API
  slug: historical-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Supported Codes API
  slug: supported-codes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Quota API
  slug: quota
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Open Access API
  slug: open-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Exchangerate Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: ExchangeRate-API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ExchangeRate-API
provider_slug: exchangerate-api
scheme_count: 1
schemes:
- description: ExchangeRate-API uses an API key embedded in the URL path (after /v6/).
  in: path
  name: apiKeyPath
  parameter: api_key
  sources:
  - openapi/exchangerate-api-openapi.yml
  type: apiKey
slug: exchangerate-api-authentication
source_filename: exchangerate-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exchangerate-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: apiKeyPath\n  type: apiKey\n  in: path\n  parameter: api_key\n  description: ExchangeRate-API uses an API key embedded in the URL path (after /v6/).\n  sources:\n  - openapi/exchangerate-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/authentication/exchangerate-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency Exchange
- Foreign Exchange
- Financial Data
- Forex
- Currency Conversion
- Public APIs
---
