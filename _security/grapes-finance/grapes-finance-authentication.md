---
api_key_in:
- header
api_specs:
- filename: grapes-finance-contacts-api-openapi.yml
  format: yaml
  label: Grapes Finance Contacts API
  slug: grapes-finance-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-contacts-api-openapi.yml
- filename: grapes-finance-kyc-api-openapi.yml
  format: yaml
  label: Grapes Finance KYC API
  slug: grapes-finance-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-kyc-api-openapi.yml
- filename: grapes-finance-orders-api-openapi.yml
  format: yaml
  label: Grapes Finance Orders API
  slug: grapes-finance-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-orders-api-openapi.yml
- filename: grapes-finance-organizations-api-openapi.yml
  format: yaml
  label: Grapes Finance Organizations API
  slug: grapes-finance-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-organizations-api-openapi.yml
- filename: grapes-finance-users-api-openapi.yml
  format: yaml
  label: Grapes Finance Users API
  slug: grapes-finance-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-users-api-openapi.yml
- filename: grapes-finance-wallets-api-openapi.yml
  format: yaml
  label: Grapes Finance Wallets API
  slug: grapes-finance-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-wallets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Grapes Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grapes Finance secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grapes Finance
provider_slug: grapes-finance
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/grapes-finance-openapi.yml
  type: apiKey
slug: grapes-finance-authentication
source_filename: grapes-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grapes-finance-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/grapes-finance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/authentication/grapes-finance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Stablecoin
- Onramp
- Offramp
- Fiat
- Payments
- Cryptocurrency
- Embedded Finance
---
