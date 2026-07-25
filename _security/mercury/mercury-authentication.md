---
api_key_in: []
api_specs:
- filename: mercury-webhooks-asyncapi.yml
  format: yaml
  label: Mercury Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/asyncapi/mercury-webhooks-asyncapi.yml
- filename: mercury-accounts-api-openapi.yml
  format: yaml
  label: Mercury Accounts API
  slug: mercury-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-accounts-api-openapi.yml
- filename: mercury-cards-api-openapi.yml
  format: yaml
  label: Mercury Cards API
  slug: mercury-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-cards-api-openapi.yml
- filename: mercury-payments-api-openapi.yml
  format: yaml
  label: Mercury Payments API
  slug: mercury-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-payments-api-openapi.yml
- filename: mercury-recipients-api-openapi.yml
  format: yaml
  label: Mercury Recipients API
  slug: mercury-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-recipients-api-openapi.yml
- filename: mercury-statements-api-openapi.yml
  format: yaml
  label: Mercury Statements API
  slug: mercury-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-statements-api-openapi.yml
- filename: mercury-transactions-api-openapi.yml
  format: yaml
  label: Mercury Transactions API
  slug: mercury-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-transactions-api-openapi.yml
- filename: mercury-treasury-api-openapi.yml
  format: yaml
  label: Mercury Treasury API
  slug: mercury-treasury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-treasury-api-openapi.yml
- filename: mercury-webhooks-api-openapi.yml
  format: yaml
  label: Mercury Webhooks API
  slug: mercury-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/openapi/mercury-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mercury Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mercury secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mercury
provider_slug: mercury
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'Mercury API token (read-only or read-and-write). Send as

    "Authorization: Bearer {token}". Read-and-write tokens require

    IP whitelisting.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mercury-openapi.yml
  type: http
slug: mercury-authentication
source_filename: mercury-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mercury-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: |-\n    Mercury API token (read-only or read-and-write). Send as\n    \"Authorization: Bearer {token}\". Read-and-write tokens require\n    IP whitelisting.\n  sources:\n  - openapi/mercury-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/authentication/mercury-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Fintech
- Startups
- Treasury
- Payments
---
