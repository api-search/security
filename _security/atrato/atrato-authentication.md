---
api_key_in:
- header
api_specs:
- filename: atrato-partners-openapi.yml
  format: yaml
  label: Atrato Partners API
  slug: atrato-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/openapi/atrato-partners-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Atrato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atrato secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Atrato
provider_slug: atrato
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: x-auth-token
  sources:
  - openapi/atrato-partners-openapi.yml
  type: apiKey
slug: atrato-authentication
source_filename: atrato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/atrato-partners-openapi.yml\ndocs: https://docs.atratopago.com/reference/autenticación\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-auth-token\n  sources:\n  - openapi/atrato-partners-openapi.yml\nflow:\n  token_endpoints:\n  - POST /api/v4/integration/login\n  - POST /api/v4/ecommerce/integration/{partner-key}/login\n  credentials: partner-dashboard username + password\n  token_ttl: 5 minutes\n  extra: Ecommerce endpoints additionally require a partner-key path segment obtained from the partner dashboard (Development > API).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/authentication/atrato-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Lending
- Mexico
- Point of Sale
- Ecommerce
---
