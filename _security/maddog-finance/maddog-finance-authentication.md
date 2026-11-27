---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: maddog-finance-access-api-openapi.yml
  format: yaml
  label: MADDOG Access API
  slug: maddog-finance-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-access-api-openapi.yml
- filename: maddog-finance-backtesting-api-openapi.yml
  format: yaml
  label: MADDOG Backtesting API
  slug: maddog-finance-backtesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-backtesting-api-openapi.yml
- filename: maddog-finance-market-data-api-openapi.yml
  format: yaml
  label: MADDOG Market data API
  slug: maddog-finance-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-market-data-api-openapi.yml
- filename: maddog-finance-market-statistics-api-openapi.yml
  format: yaml
  label: MADDOG Market statistics API
  slug: maddog-finance-market-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-market-statistics-api-openapi.yml
- filename: maddog-finance-service-api-openapi.yml
  format: yaml
  label: MADDOG Service API
  slug: maddog-finance-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-service-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MADDOG Authentication
name_suffix: Authentication
oauth_flows: []
overview: MADDOG secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MADDOG
provider_slug: maddog-finance
scheme_count: 1
schemes:
- description: API key, starts with qd_. Request a free key by email at POST /v1/access/free-key — no card, no account. Full access is $99.9/month with a 3-day free trial. Missing or invalid keys get a problem+json body with machine-readable free-key and checkout actions.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/maddog-finance-openapi.json
  type: apiKey
slug: maddog-finance-authentication
source_filename: maddog-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/maddog-finance-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key, starts with qd_. Request a free key by email at POST /v1/access/free-key\n    — no card, no account. Full access is $99.9/month with a 3-day free trial. Missing or invalid\n    keys get a problem+json body with machine-readable free-key and checkout actions.\n  sources:\n  - openapi/maddog-finance-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/maddog-finance/authentication/maddog-finance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Trading
- Finance
- Analytics
- Price-Action
---
