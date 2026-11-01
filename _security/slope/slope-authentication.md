---
anonymous_access: false
api_key_in: []
api_specs:
- filename: slope-auth-api-openapi.yml
  format: yaml
  label: Slope Auth API
  slug: slope-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-auth-api-openapi.yml
- filename: slope-customers-api-openapi.yml
  format: yaml
  label: Slope Customers API
  slug: slope-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-customers-api-openapi.yml
- filename: slope-files-api-openapi.yml
  format: yaml
  label: Slope Files API
  slug: slope-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-files-api-openapi.yml
- filename: slope-orders-api-openapi.yml
  format: yaml
  label: Slope Orders API
  slug: slope-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-orders-api-openapi.yml
- filename: slope-payout-accounts-api-openapi.yml
  format: yaml
  label: Slope Payout Accounts API
  slug: slope-payout-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-payout-accounts-api-openapi.yml
- filename: slope-persons-api-openapi.yml
  format: yaml
  label: Slope Persons API
  slug: slope-persons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-persons-api-openapi.yml
- filename: slope-prescreens-api-openapi.yml
  format: yaml
  label: Slope Prescreens API
  slug: slope-prescreens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-prescreens-api-openapi.yml
- filename: slope-simulation-api-openapi.yml
  format: yaml
  label: Slope Simulation API
  slug: slope-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-simulation-api-openapi.yml
- filename: slope-transactions-api-openapi.yml
  format: yaml
  label: Slope Transactions API
  slug: slope-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-transactions-api-openapi.yml
- filename: slope-user-links-api-openapi.yml
  format: yaml
  label: Slope User Links API
  slug: slope-user-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slope/openapi/slope-user-links-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Slope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slope secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slope
provider_slug: slope
scheme_count: 1
schemes:
- description: Basic HTTP authentication using the base64 hash of `public_key:secret_key`.
  name: apiKey
  scheme: basic
  sources:
  - openapi/slope-v4-openapi.json
  type: http
slug: slope-authentication
source_filename: slope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/slope-v4-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: Basic HTTP authentication using the base64 hash of `public_key:secret_key`.\n  sources:\n  - openapi/slope-v4-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/slope/authentication/slope-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Buy Now Pay Later
- Lending
- Credit
- B2B
- Checkout
---
