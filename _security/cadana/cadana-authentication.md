---
api_key_in: []
api_specs:
- filename: cadana-workforce-management-openapi.yaml
  format: yaml
  label: Business Workforce Management
  slug: business-workforce-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-workforce-management-openapi.yaml
- filename: cadana-embedded-payments-openapi.yaml
  format: yaml
  label: Embedded Payments
  slug: embedded-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-embedded-payments-openapi.yaml
- filename: cadana-embedded-consumer-wallets-openapi.yaml
  format: yaml
  label: Embedded Consumer Wallets
  slug: embedded-consumer-wallets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-embedded-consumer-wallets-openapi.yaml
- filename: cadana-global-tax-openapi.yaml
  format: yaml
  label: Global Tax Engine
  slug: global-tax-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-global-tax-openapi.yaml
- filename: cadana-statutory-compliance-openapi.yaml
  format: yaml
  label: Statutory Compliance API
  slug: statutory-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-statutory-compliance-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cadana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cadana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cadana
provider_slug: cadana
scheme_count: 1
schemes:
- bearerFormat: API_SECRET_KEY
  name: Authorization
  scheme: bearer
  sources:
  - openapi/cadana-embedded-consumer-wallets-openapi.yaml
  - openapi/cadana-embedded-payments-openapi.yaml
  - openapi/cadana-global-tax-openapi.yaml
  - openapi/cadana-statutory-compliance-openapi.yaml
  - openapi/cadana-workforce-management-openapi.yaml
  type: http
slug: cadana-authentication
source_filename: cadana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cadana-embedded-consumer-wallets-openapi.yaml, openapi/cadana-embedded-payments-openapi.yaml,\n  openapi/cadana-global-tax-openapi.yaml, openapi/cadana-statutory-compliance-openapi.yaml,\n  openapi/cadana-workforce-management-openapi.yaml\ndocs: https://docs.cadanapay.com/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer\n  header: 'Authorization: Bearer <API_KEY>'\n  verify_operation: getMe\n  verify_endpoint: GET /v1/me\ntoken_types:\n- name: Org Token\n  scope: single organization\n  expiration: none\n  use: backend integrations\n- name: Platform Token\n  scope: multiple businesses (multi-tenant)\n  expiration: none\n  use: multi-tenant platforms\n  extra_header: 'X-MultiTenantKey: <tenantKey>'\n  notes: Tenant key is returned when you create a business; omitting it defaults to\n    the primary platform business.\n- name: User Token\n  scope: single user\n  expiration: 1 hour\n  use: frontend / mobile\
  \ apps\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  bearerFormat: API_SECRET_KEY\n  sources:\n  - openapi/cadana-embedded-consumer-wallets-openapi.yaml\n  - openapi/cadana-embedded-payments-openapi.yaml\n  - openapi/cadana-global-tax-openapi.yaml\n  - openapi/cadana-statutory-compliance-openapi.yaml\n  - openapi/cadana-workforce-management-openapi.yaml\nerrors:\n  '401': missing or invalid token\n  '403': insufficient permissions or incorrect tenant key (Platform tokens)\ncustom_auth:\n  jwt_exchange_operation: exchangeJwtToken\n  jwt_exchange_endpoint: POST /v1/auth/login/jwt\n  docs: https://docs.cadanapay.com/white-label/custom-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/authentication/cadana-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payroll
- Payments
- Global Payroll
- Contractor Payments
- Embedded Finance
- Wallets
- Tax
- Compliance
- Fintech
- Money Transfer
- White Label
---
