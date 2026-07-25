---
api_key_in: []
api_specs:
- filename: quaderno-authentication-api-openapi.yml
  format: yaml
  label: Quaderno Authentication API
  slug: quaderno-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-authentication-api-openapi.yml
- filename: quaderno-checkout-api-openapi.yml
  format: yaml
  label: Quaderno Checkout API
  slug: quaderno-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-checkout-api-openapi.yml
- filename: quaderno-contacts-api-openapi.yml
  format: yaml
  label: Quaderno Contacts API
  slug: quaderno-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-contacts-api-openapi.yml
- filename: quaderno-credits-api-openapi.yml
  format: yaml
  label: Quaderno Credits API
  slug: quaderno-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-credits-api-openapi.yml
- filename: quaderno-estimates-api-openapi.yml
  format: yaml
  label: Quaderno Estimates API
  slug: quaderno-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-estimates-api-openapi.yml
- filename: quaderno-evidences-api-openapi.yml
  format: yaml
  label: Quaderno Evidences API
  slug: quaderno-evidences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-evidences-api-openapi.yml
- filename: quaderno-expenses-api-openapi.yml
  format: yaml
  label: Quaderno Expenses API
  slug: quaderno-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-expenses-api-openapi.yml
- filename: quaderno-invoices-api-openapi.yml
  format: yaml
  label: Quaderno Invoices API
  slug: quaderno-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-invoices-api-openapi.yml
- filename: quaderno-items-api-openapi.yml
  format: yaml
  label: Quaderno Items API
  slug: quaderno-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-items-api-openapi.yml
- filename: quaderno-payments-api-openapi.yml
  format: yaml
  label: Quaderno Payments API
  slug: quaderno-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-payments-api-openapi.yml
- filename: quaderno-recurring-api-openapi.yml
  format: yaml
  label: Quaderno Recurring API
  slug: quaderno-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-recurring-api-openapi.yml
- filename: quaderno-taxes-api-openapi.yml
  format: yaml
  label: Quaderno Taxes API
  slug: quaderno-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-taxes-api-openapi.yml
- filename: quaderno-transactions-api-openapi.yml
  format: yaml
  label: Quaderno Transactions API
  slug: quaderno-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-transactions-api-openapi.yml
- filename: quaderno-webhooks-api-openapi.yml
  format: yaml
  label: Quaderno Webhooks API
  slug: quaderno-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-webhooks-api-openapi.yml
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
