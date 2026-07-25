---
api_key_in: []
api_specs:
- filename: highline-fi-auth-api-openapi.yml
  format: yaml
  label: Highline Auth API
  slug: highline-fi-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-auth-api-openapi.yml
- filename: highline-fi-companies-api-openapi.yml
  format: yaml
  label: Highline Companies API
  slug: highline-fi-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-companies-api-openapi.yml
- filename: highline-fi-connections-api-openapi.yml
  format: yaml
  label: Highline Connections API
  slug: highline-fi-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-connections-api-openapi.yml
- filename: highline-fi-employments-api-openapi.yml
  format: yaml
  label: Highline Employments API
  slug: highline-fi-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-employments-api-openapi.yml
- filename: highline-fi-payment-requests-api-openapi.yml
  format: yaml
  label: Highline Payment Requests API
  slug: highline-fi-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-payment-requests-api-openapi.yml
- filename: highline-fi-payments-api-openapi.yml
  format: yaml
  label: Highline Payments API
  slug: highline-fi-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-payments-api-openapi.yml
- filename: highline-fi-products-api-openapi.yml
  format: yaml
  label: Highline Products API
  slug: highline-fi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-products-api-openapi.yml
- filename: highline-fi-settlements-api-openapi.yml
  format: yaml
  label: Highline Settlements API
  slug: highline-fi-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-settlements-api-openapi.yml
- filename: highline-fi-users-api-openapi.yml
  format: yaml
  label: Highline Users API
  slug: highline-fi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Highline Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highline secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highline
provider_slug: highline-fi
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/highline-fi-openapi.yml
  type: http
slug: highline-fi-authentication
source_filename: highline-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/highline-fi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/highline-fi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/authentication/highline-fi-authentication.yml
summary_line: http · 1 scheme
tags:
- Embedded Finance
- Payroll
- Payments
- ACH
- Bill Pay
- Lending
- Direct Deposit
- API-First
- Webhooks
- Pay by Paycheck
---
