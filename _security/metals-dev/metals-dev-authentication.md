---
api_key_in:
- query
api_specs:
- filename: metals-dev-account-api-openapi.yml
  format: yaml
  label: Metals.Dev Account API
  slug: metals-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-account-api-openapi.yml
- filename: metals-dev-authority-api-openapi.yml
  format: yaml
  label: Metals.Dev Authority API
  slug: metals-dev-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-authority-api-openapi.yml
- filename: metals-dev-currency-api-openapi.yml
  format: yaml
  label: Metals.Dev Currency API
  slug: metals-dev-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-currency-api-openapi.yml
- filename: metals-dev-rates-api-openapi.yml
  format: yaml
  label: Metals.Dev Rates API
  slug: metals-dev-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-rates-api-openapi.yml
- filename: metals-dev-spot-prices-api-openapi.yml
  format: yaml
  label: Metals.Dev Spot Prices API
  slug: metals-dev-spot-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-spot-prices-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metals Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metals.Dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metals.Dev
provider_slug: metals-dev
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/metals-dev-openapi.yml
  type: apiKey
slug: metals-dev-authentication
source_filename: metals-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metals-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/metals-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/authentication/metals-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Data
- Gold
- Precious Metals
- Silver
- Spot Prices
---
