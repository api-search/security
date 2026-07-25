---
api_key_in: []
api_specs:
- filename: avaloq-accounts-api-openapi.yml
  format: yaml
  label: Avaloq Accounts API
  slug: avaloq-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-accounts-api-openapi.yml
- filename: avaloq-customers-api-openapi.yml
  format: yaml
  label: Avaloq Customers API
  slug: avaloq-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-customers-api-openapi.yml
- filename: avaloq-payment-status-api-openapi.yml
  format: yaml
  label: Avaloq Payment Status API
  slug: avaloq-payment-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-payment-status-api-openapi.yml
- filename: avaloq-payments-api-openapi.yml
  format: yaml
  label: Avaloq Payments API
  slug: avaloq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-payments-api-openapi.yml
- filename: avaloq-transactions-api-openapi.yml
  format: yaml
  label: Avaloq Transactions API
  slug: avaloq-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Avaloq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avaloq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avaloq
provider_slug: avaloq
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avaloq-banking-openapi.yml
  - openapi/avaloq-payments-openapi.yml
  type: http
slug: avaloq-authentication
source_filename: avaloq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/avaloq-banking-openapi.yml, openapi/avaloq-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/avaloq-banking-openapi.yml\n  - openapi/avaloq-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/authentication/avaloq-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
---
