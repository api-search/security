---
api_key_in: []
api_specs:
- filename: temenos-transact-accounts-api-openapi.yml
  format: yaml
  label: Temenos Transact Accounts API
  slug: temenos-transact-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-accounts-api-openapi.yml
- filename: temenos-transact-beneficiaries-api-openapi.yml
  format: yaml
  label: Temenos Transact Beneficiaries API
  slug: temenos-transact-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-beneficiaries-api-openapi.yml
- filename: temenos-transact-cards-api-openapi.yml
  format: yaml
  label: Temenos Transact Cards API
  slug: temenos-transact-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-cards-api-openapi.yml
- filename: temenos-transact-customers-api-openapi.yml
  format: yaml
  label: Temenos Transact Customers API
  slug: temenos-transact-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-customers-api-openapi.yml
- filename: temenos-transact-deposits-api-openapi.yml
  format: yaml
  label: Temenos Transact Deposits API
  slug: temenos-transact-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-deposits-api-openapi.yml
- filename: temenos-transact-loans-api-openapi.yml
  format: yaml
  label: Temenos Transact Loans API
  slug: temenos-transact-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-loans-api-openapi.yml
- filename: temenos-transact-payments-api-openapi.yml
  format: yaml
  label: Temenos Transact Payments API
  slug: temenos-transact-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-payments-api-openapi.yml
- filename: temenos-transact-products-api-openapi.yml
  format: yaml
  label: Temenos Transact Products API
  slug: temenos-transact-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-products-api-openapi.yml
- filename: temenos-transact-reference-data-api-openapi.yml
  format: yaml
  label: Temenos Transact Reference Data API
  slug: temenos-transact-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-reference-data-api-openapi.yml
- filename: temenos-transact-transactions-api-openapi.yml
  format: yaml
  label: Temenos Transact Transactions API
  slug: temenos-transact-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Temenos Transact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temenos Transact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Temenos Transact
provider_slug: temenos-transact
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token authentication. Obtain a token from the Temenos authentication endpoint using client credentials or authorization code flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/temenos-transact-core-banking-openapi.yml
  type: http
slug: temenos-transact-authentication
source_filename: temenos-transact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temenos-transact-core-banking-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token authentication. Obtain a token from the Temenos authentication\n    endpoint using client credentials or authorization code flow.\n  sources:\n  - openapi/temenos-transact-core-banking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/authentication/temenos-transact-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
---
