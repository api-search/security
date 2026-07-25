---
api_key_in: []
api_specs:
- filename: treasury-prime-accounts-api-openapi.yml
  format: yaml
  label: Treasury Prime Accounts API
  slug: treasury-prime-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-accounts-api-openapi.yml
- filename: treasury-prime-businesses-api-openapi.yml
  format: yaml
  label: Treasury Prime Businesses API
  slug: treasury-prime-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-businesses-api-openapi.yml
- filename: treasury-prime-cards-api-openapi.yml
  format: yaml
  label: Treasury Prime Cards API
  slug: treasury-prime-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-cards-api-openapi.yml
- filename: treasury-prime-health-api-openapi.yml
  format: yaml
  label: Treasury Prime Health API
  slug: treasury-prime-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-health-api-openapi.yml
- filename: treasury-prime-payments-api-openapi.yml
  format: yaml
  label: Treasury Prime Payments API
  slug: treasury-prime-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-payments-api-openapi.yml
- filename: treasury-prime-persons-api-openapi.yml
  format: yaml
  label: Treasury Prime Persons API
  slug: treasury-prime-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-persons-api-openapi.yml
- filename: treasury-prime-statements-api-openapi.yml
  format: yaml
  label: Treasury Prime Statements API
  slug: treasury-prime-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-statements-api-openapi.yml
- filename: treasury-prime-transactions-api-openapi.yml
  format: yaml
  label: Treasury Prime Transactions API
  slug: treasury-prime-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-transactions-api-openapi.yml
- filename: treasury-prime-webhooks-api-openapi.yml
  format: yaml
  label: Treasury Prime Webhooks API
  slug: treasury-prime-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Treasury Prime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treasury Prime secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Treasury Prime
provider_slug: treasury-prime
scheme_count: 1
schemes:
- description: HTTP Basic Auth using API Key ID (username) and Secret (password).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/treasury-prime-openapi.yml
  type: http
slug: treasury-prime-authentication
source_filename: treasury-prime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/treasury-prime-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using API Key ID (username) and Secret (password).\n  sources:\n  - openapi/treasury-prime-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/authentication/treasury-prime-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
---
