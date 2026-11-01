---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: track-accounts-api-openapi.yml
  format: yaml
  label: Track Accounts API
  slug: track-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-accounts-api-openapi.yml
- filename: track-catalogue-api-openapi.yml
  format: yaml
  label: Track Catalogue API
  slug: track-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-catalogue-api-openapi.yml
- filename: track-contracts-api-openapi.yml
  format: yaml
  label: Track Contracts API
  slug: track-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-contracts-api-openapi.yml
- filename: track-expenses-api-openapi.yml
  format: yaml
  label: Track Expenses API
  slug: track-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-expenses-api-openapi.yml
- filename: track-imports-api-openapi.yml
  format: yaml
  label: Track Imports API
  slug: track-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-imports-api-openapi.yml
- filename: track-ledger-api-openapi.yml
  format: yaml
  label: Track Ledger API
  slug: track-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-ledger-api-openapi.yml
- filename: track-payments-api-openapi.yml
  format: yaml
  label: Track Payments API
  slug: track-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-payments-api-openapi.yml
- filename: track-portal-api-openapi.yml
  format: yaml
  label: Track Portal API
  slug: track-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-portal-api-openapi.yml
- filename: track-revenue-api-openapi.yml
  format: yaml
  label: Track Revenue API
  slug: track-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-revenue-api-openapi.yml
- filename: track-open-api-api-openapi.yml
  format: yaml
  label: Track Open API
  slug: track-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/track/openapi/track-open-api-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Track Authentication
name_suffix: Authentication
oauth_flows: []
overview: Track secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Track
provider_slug: track
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/track-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/track-openapi.yml
  type: http
slug: track-authentication
source_filename: track-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/track-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/track-openapi.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/track-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/track/authentication/track-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Music
- FinTech
- Royalties
- Payments
- Banking
- API
---
