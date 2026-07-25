---
api_key_in: []
api_specs:
- filename: instamojo-authentication-api-openapi.yml
  format: yaml
  label: Instamojo Authentication API
  slug: instamojo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-authentication-api-openapi.yml
- filename: instamojo-orders-api-openapi.yml
  format: yaml
  label: Instamojo Orders API
  slug: instamojo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-orders-api-openapi.yml
- filename: instamojo-payment-requests-api-openapi.yml
  format: yaml
  label: Instamojo Payment Requests API
  slug: instamojo-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-payment-requests-api-openapi.yml
- filename: instamojo-payments-api-openapi.yml
  format: yaml
  label: Instamojo Payments API
  slug: instamojo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-payments-api-openapi.yml
- filename: instamojo-refunds-api-openapi.yml
  format: yaml
  label: Instamojo Refunds API
  slug: instamojo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-refunds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Instamojo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instamojo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instamojo
provider_slug: instamojo
scheme_count: 1
schemes:
- description: OAuth2 Bearer token obtained from /oauth2/token/
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/instamojo-payments-api.yml
  type: http
slug: instamojo-authentication
source_filename: instamojo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instamojo-payments-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer token obtained from /oauth2/token/\n  sources:\n  - openapi/instamojo-payments-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/authentication/instamojo-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- E-Commerce
- India
- Payment Gateway
- Payment Links
- Refunds
- Orders
---
