---
api_key_in: []
api_specs:
- filename: conekta-api-openapi.yml
  format: yaml
  label: Conekta API
  slug: conekta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conekta/refs/heads/main/openapi/conekta-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Conekta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conekta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Conekta
provider_slug: conekta
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/conekta-api-openapi.yml
  type: http
slug: conekta-authentication
source_filename: conekta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/conekta-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/conekta-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conekta/refs/heads/main/authentication/conekta-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Processing
- Cards
- Cash
- OXXO
- SPEI
- Mexico
- Latin America
- LATAM
- Fintech
- Subscriptions
- Antifraud
- Checkout
- BNPL
- 3D Secure
---
