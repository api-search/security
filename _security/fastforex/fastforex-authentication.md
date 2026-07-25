---
api_key_in:
- header
- query
api_specs:
- filename: fastforex-admin-api-openapi.yml
  format: yaml
  label: FastForex admin API
  slug: fastforex-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-admin-api-openapi.yml
- filename: fastforex-crypto-api-openapi.yml
  format: yaml
  label: FastForex crypto API
  slug: fastforex-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-crypto-api-openapi.yml
- filename: fastforex-currency-api-openapi.yml
  format: yaml
  label: FastForex currency API
  slug: fastforex-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-currency-api-openapi.yml
- filename: fastforex-fx-api-openapi.yml
  format: yaml
  label: FastForex fx API
  slug: fastforex-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-fx-api-openapi.yml
- filename: fastforex-plan-extra-api-openapi.yml
  format: yaml
  label: FastForex plan-extra API
  slug: fastforex-plan-extra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-extra-api-openapi.yml
- filename: fastforex-plan-one-api-openapi.yml
  format: yaml
  label: FastForex plan-one API
  slug: fastforex-plan-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-one-api-openapi.yml
- filename: fastforex-plan-premium-api-openapi.yml
  format: yaml
  label: FastForex plan-premium API
  slug: fastforex-plan-premium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-premium-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fastforex Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastForex secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FastForex
provider_slug: fastforex
scheme_count: 4
schemes:
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/openapi.yaml
  type: apiKey
- in: header
  name: apiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yaml
  type: apiKey
- bearerFormat: api_key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yaml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/openapi.yaml
  type: http
slug: fastforex-authentication
source_filename: fastforex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/openapi.yaml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: api_key\n  sources:\n  - openapi/openapi.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/authentication/fastforex-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Currency Exchange
- Forex
- Financial Data
- Exchange Rates
- Cryptocurrency
- FX Trading
- Historical Data
- Real-Time Data
---
