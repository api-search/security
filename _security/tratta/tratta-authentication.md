---
api_key_in: []
api_specs:
- filename: tratta-bulk-operations-api-openapi.yml
  format: yaml
  label: Tratta Bulk Operations API
  slug: tratta-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-bulk-operations-api-openapi.yml
- filename: tratta-charges-api-openapi.yml
  format: yaml
  label: Tratta Charges API
  slug: tratta-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-charges-api-openapi.yml
- filename: tratta-customer-sessions-api-openapi.yml
  format: yaml
  label: Tratta Customer Sessions API
  slug: tratta-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-customer-sessions-api-openapi.yml
- filename: tratta-customers-api-openapi.yml
  format: yaml
  label: Tratta Customers API
  slug: tratta-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-customers-api-openapi.yml
- filename: tratta-debt-accounts-api-openapi.yml
  format: yaml
  label: Tratta Debt Accounts API
  slug: tratta-debt-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-debt-accounts-api-openapi.yml
- filename: tratta-payment-methods-api-openapi.yml
  format: yaml
  label: Tratta Payment Methods API
  slug: tratta-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-payment-methods-api-openapi.yml
- filename: tratta-payment-plans-api-openapi.yml
  format: yaml
  label: Tratta Payment Plans API
  slug: tratta-payment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-payment-plans-api-openapi.yml
- filename: tratta-tickets-api-openapi.yml
  format: yaml
  label: Tratta Tickets API
  slug: tratta-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-tickets-api-openapi.yml
- filename: tratta-transactions-api-openapi.yml
  format: yaml
  label: Tratta Transactions API
  slug: tratta-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-transactions-api-openapi.yml
- filename: tratta-webhooks-api-openapi.yml
  format: yaml
  label: Tratta Webhooks API
  slug: tratta-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tratta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tratta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tratta
provider_slug: tratta
scheme_count: 1
schemes:
- description: Bearer token provided by Tratta after organization setup
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tratta-openapi.yml
  type: http
slug: tratta-authentication
source_filename: tratta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tratta-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token provided by Tratta after organization setup\n  sources:\n  - openapi/tratta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/authentication/tratta-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Collection
- Payments
- Debt Collection
- Fintech
---
