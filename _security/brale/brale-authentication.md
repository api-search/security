---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brale-accounts-api-openapi.yml
  format: yaml
  label: Brale Accounts API
  slug: brale-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-accounts-api-openapi.yml
- filename: brale-addresses-api-openapi.yml
  format: yaml
  label: Brale Addresses API
  slug: brale-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-addresses-api-openapi.yml
- filename: brale-automations-api-openapi.yml
  format: yaml
  label: Brale Automations API
  slug: brale-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-automations-api-openapi.yml
- filename: brale-financial-institutions-api-openapi.yml
  format: yaml
  label: Brale Financial Institutions API
  slug: brale-financial-institutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-financial-institutions-api-openapi.yml
- filename: brale-orders-api-openapi.yml
  format: yaml
  label: Brale Orders API
  slug: brale-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-orders-api-openapi.yml
- filename: brale-plaid-api-openapi.yml
  format: yaml
  label: Brale Plaid API
  slug: brale-plaid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-plaid-api-openapi.yml
- filename: brale-transfers-api-openapi.yml
  format: yaml
  label: Brale Transfers API
  slug: brale-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brale/openapi/brale-transfers-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Brale Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Brale secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Brale
provider_slug: brale
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 11
    tokenUrl: https://auth.brale.xyz/oauth2/token
  name: oauth
  sources:
  - openapi/brale-openapi-original.yml
  type: oauth2
slug: brale-authentication
source_filename: brale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brale-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.brale.xyz/oauth2/token\n    scopes: 11\n  sources:\n  - openapi/brale-openapi-original.yml\n"
source_yaml_url: https://artifacts.apis.io/brale/authentication/brale-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Stablecoins
- Stablecoin Issuance
- Payments
- Blockchain
- Cryptocurrency
- Fintech
- Financial Services
- Custody
- Tokenization
- On-Ramp
- Off-Ramp
- A2A
---
