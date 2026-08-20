---
api_key_in: []
api_specs:
- filename: column-ach-transfers-api-openapi.yml
  format: yaml
  label: Column ACH Transfers API
  slug: column-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-ach-transfers-api-openapi.yml
- filename: column-wire-transfers-api-openapi.yml
  format: yaml
  label: Column Wire Transfers API
  slug: column-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-wire-transfers-api-openapi.yml
- filename: column-international-wires-api-openapi.yml
  format: yaml
  label: Column International Wires API
  slug: column-international-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-international-wires-api-openapi.yml
- filename: column-realtime-transfers-api-openapi.yml
  format: yaml
  label: Column Realtime Transfers API
  slug: column-realtime-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-realtime-transfers-api-openapi.yml
- filename: column-book-transfers-api-openapi.yml
  format: yaml
  label: Column Book Transfers API
  slug: column-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-book-transfers-api-openapi.yml
- filename: column-asyncapi.yml
  format: yaml
  label: Column Webhooks
  slug: column-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-asyncapi.yml
- filename: column-account-numbers-api-openapi.yml
  format: yaml
  label: Column Account Numbers API
  slug: column-account-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-account-numbers-api-openapi.yml
- filename: column-ach-transfers-api-openapi.yml
  format: yaml
  label: Column ACH Transfers API
  slug: column-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-ach-transfers-api-openapi.yml
- filename: column-bank-accounts-api-openapi.yml
  format: yaml
  label: Column Bank Accounts API
  slug: column-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-bank-accounts-api-openapi.yml
- filename: column-book-transfers-api-openapi.yml
  format: yaml
  label: Column Book Transfers API
  slug: column-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-book-transfers-api-openapi.yml
- filename: column-check-transfers-api-openapi.yml
  format: yaml
  label: Column Check Transfers API
  slug: column-check-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-check-transfers-api-openapi.yml
- filename: column-counterparties-api-openapi.yml
  format: yaml
  label: Column Counterparties API
  slug: column-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-counterparties-api-openapi.yml
- filename: column-entities-api-openapi.yml
  format: yaml
  label: Column Entities API
  slug: column-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-entities-api-openapi.yml
- filename: column-events-api-openapi.yml
  format: yaml
  label: Column Events API
  slug: column-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-events-api-openapi.yml
- filename: column-international-wires-api-openapi.yml
  format: yaml
  label: Column International Wires API
  slug: column-international-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-international-wires-api-openapi.yml
- filename: column-realtime-transfers-api-openapi.yml
  format: yaml
  label: Column Realtime Transfers API
  slug: column-realtime-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-realtime-transfers-api-openapi.yml
- filename: column-webhooks-api-openapi.yml
  format: yaml
  label: Column Webhooks API
  slug: column-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-webhooks-api-openapi.yml
- filename: column-wire-transfers-api-openapi.yml
  format: yaml
  label: Column Wire Transfers API
  slug: column-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-wire-transfers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Column Authentication
name_suffix: Authentication
oauth_flows: []
overview: Column secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Column
provider_slug: column
scheme_count: 1
schemes:
- description: Column uses HTTP Basic Auth with your API key as the username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/column-openapi.yml
  type: http
slug: column-authentication
source_filename: column-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/column-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Column uses HTTP Basic Auth with your API key as the username.\n  sources:\n  - openapi/column-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/authentication/column-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Banking
- Backend-as-a-Service
- ACH
- Wires
---
