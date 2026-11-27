---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: leakdata-io-alerts-api-openapi.yml
  format: yaml
  label: LeakData Alerts API
  slug: leakdata-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-alerts-api-openapi.yml
- filename: leakdata-io-domains-api-openapi.yml
  format: yaml
  label: LeakData Domains API
  slug: leakdata-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-domains-api-openapi.yml
- filename: leakdata-io-easm-api-openapi.yml
  format: yaml
  label: LeakData EASM API
  slug: leakdata-io-easm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-easm-api-openapi.yml
- filename: leakdata-io-password-api-openapi.yml
  format: yaml
  label: LeakData Password API
  slug: leakdata-io-password-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-password-api-openapi.yml
- filename: leakdata-io-search-api-openapi.yml
  format: yaml
  label: LeakData Search API
  slug: leakdata-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-search-api-openapi.yml
- filename: leakdata-io-social-api-openapi.yml
  format: yaml
  label: LeakData Social API
  slug: leakdata-io-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-social-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: LeakData Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeakData secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeakData
provider_slug: leakdata-io
scheme_count: 2
schemes:
- bearerFormat: LeakData API key
  description: Requires an active, email-verified key owner with API entitlement. Read-only seat accounts cannot use API keys. Access is denied while account data deletion is in progress.
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/leakdata-io-openapi.json
  type: http
- description: Requires an active, email-verified key owner with API entitlement. Read-only seat accounts cannot use API keys. Access is denied while account data deletion is in progress.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/leakdata-io-openapi.json
  type: apiKey
slug: leakdata-io-authentication
source_filename: leakdata-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/leakdata-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: LeakData API key\n  description: Requires an active, email-verified key owner with API entitlement. Read-only\n    seat accounts cannot use API keys. Access is denied while account data deletion is in progress.\n  sources:\n  - openapi/leakdata-io-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Requires an active, email-verified key owner with API entitlement. Read-only\n    seat accounts cannot use API keys. Access is denied while account data deletion is in progress.\n  sources:\n  - openapi/leakdata-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/leakdata-io/authentication/leakdata-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Breaches
- Digital Risk
- Cybersecurity
- Monitoring
- Intelligence
---
