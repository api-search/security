---
api_key_in: []
api_specs:
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Checkout API
  slug: tabby-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Payments API
  slug: tabby-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Webhooks API
  slug: tabby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Disputes API
  slug: tabby-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tabby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabby secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tabby
provider_slug: tabby
scheme_count: 1
schemes:
- description: Bearer authentication header of the form `Bearer <secret_key>`, where `<secret_key>` is your `secret_key`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tabby-api-openapi.yml
  type: http
slug: tabby-authentication
source_filename: tabby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tabby-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication header of the form `Bearer <secret_key>`, where `<secret_key>`\n    is your `secret_key`.\n  sources:\n  - openapi/tabby-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/authentication/tabby-authentication.yml
summary_line: http · 1 scheme
tags:
- BNPL
- Buy Now Pay Later
- Consumer Finance
- E-commerce
- Fintech
- Installments
- MENA
- Payments
- Saudi Arabia
- UAE
---
