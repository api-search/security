---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Paidy Payments API
  slug: paidy-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/openapi/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Paidy Tokens API
  slug: paidy-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paidy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paidy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paidy
provider_slug: paidy
scheme_count: 1
schemes:
- description: Use your Paidy secret key (prefixed with `sk_`) as the bearer token. Never share your secret key. Use test keys for sandbox testing.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: paidy-authentication
source_filename: paidy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Use your Paidy secret key (prefixed with `sk_`) as the bearer token. Never share\n    your secret key. Use test keys for sandbox testing.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/authentication/paidy-authentication.yml
summary_line: http · 1 scheme
tags:
- Buy Now Pay Later
- BNPL
- Payments
- Japan
- Checkout
- Deferred Payments
- Recurring Payments
- Tokens
---
