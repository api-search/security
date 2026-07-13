---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Payflex Merchant API
  slug: payflex-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payflex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payflex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Payflex
provider_slug: payflex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer token obtained from the /auth/merchant endpoint using the client_credentials grant. Tokens expire and should be refreshed automatically before expiry.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: payflex-authentication
source_filename: payflex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer token obtained from the /auth/merchant endpoint using the client_credentials\n    grant. Tokens expire and should be refreshed automatically before expiry.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/authentication/payflex-authentication.yml
summary_line: http · 1 scheme
tags:
- BNPL
- Buy Now Pay Later
- Payments
- Installments
- South Africa
- Fintech
- E-commerce
---
