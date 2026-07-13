---
api_key_in: []
api_specs:
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Payments API
  slug: modern-treasury-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Ledgers API
  slug: modern-treasury-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Counterparties API
  slug: modern-treasury-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Connections & Webhooks API
  slug: modern-treasury-connections-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Modern Treasury Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modern Treasury secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Modern Treasury
provider_slug: modern-treasury
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/modern-treasury-openapi.yml
  type: http
slug: modern-treasury-authentication
source_filename: modern-treasury-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/modern-treasury-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/modern-treasury-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/authentication/modern-treasury-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Payments
- ACH
- Wires
- Treasury
---
