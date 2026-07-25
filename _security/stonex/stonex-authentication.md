---
api_key_in: []
api_specs:
- filename: stonex-accounts-api-openapi.yml
  format: yaml
  label: StoneX Accounts API
  slug: stonex-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-accounts-api-openapi.yml
- filename: stonex-authentication-api-openapi.yml
  format: yaml
  label: StoneX Authentication API
  slug: stonex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-authentication-api-openapi.yml
- filename: stonex-documents-api-openapi.yml
  format: yaml
  label: StoneX Documents API
  slug: stonex-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-documents-api-openapi.yml
- filename: stonex-fx-rates-api-openapi.yml
  format: yaml
  label: StoneX FX Rates API
  slug: stonex-fx-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-fx-rates-api-openapi.yml
- filename: stonex-payments-api-openapi.yml
  format: yaml
  label: StoneX Payments API
  slug: stonex-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-payments-api-openapi.yml
- filename: stonex-trading-api-openapi.yml
  format: yaml
  label: StoneX Trading API
  slug: stonex-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-trading-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stonex Authentication
name_suffix: Authentication
oauth_flows: []
overview: StoneX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StoneX
provider_slug: stonex
scheme_count: 1
schemes:
- description: JWT token from /auth/token endpoint. Valid for 10 hours.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stonex-clearing-openapi.yml
  - openapi/stonex-payments-openapi.yml
  type: http
slug: stonex-authentication
source_filename: stonex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stonex-clearing-openapi.yml, openapi/stonex-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: JWT token from /auth/token endpoint. Valid for 10 hours.\n  sources:\n  - openapi/stonex-clearing-openapi.yml\n  - openapi/stonex-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/authentication/stonex-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Financial Services
- Payments
- Clearing
- Futures
- Trading
- Risk Management
---
