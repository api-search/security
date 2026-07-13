---
api_key_in: []
api_specs:
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Invoices API
  slug: quaderno-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Credits API
  slug: quaderno-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Estimates API
  slug: quaderno-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Expenses API
  slug: quaderno-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Contacts API
  slug: quaderno-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Items API
  slug: quaderno-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Taxes API
  slug: quaderno-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Payments API
  slug: quaderno-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Transactions API
  slug: quaderno-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Checkout API
  slug: quaderno-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Webhooks API
  slug: quaderno-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quaderno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quaderno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quaderno
provider_slug: quaderno
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Use your private API key as the username; the password can be any value. API keys are managed in the Quaderno account settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/quaderno-openapi.yml
  type: http
slug: quaderno-authentication
source_filename: quaderno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quaderno-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Use your private API key as the username; the password\n    can be any value. API keys are managed in the Quaderno account settings.\n  sources:\n  - openapi/quaderno-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/authentication/quaderno-authentication.yml
summary_line: http · 1 scheme
tags:
- Tax Compliance
- Sales Tax
- VAT
- Invoicing
- Billing
- FinTech
---
