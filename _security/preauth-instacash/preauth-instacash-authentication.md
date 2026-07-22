---
api_key_in:
- header
api_specs:
- filename: preauth-instacash-orders-openapi.yml
  format: yaml
  label: Preauth Orders API
  slug: preauth-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preauth-instacash/refs/heads/main/openapi/preauth-instacash-orders-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Preauth Instacash Authentication
name_suffix: Authentication
oauth_flows: []
overview: PreAuth (Instacash) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PreAuth (Instacash)
provider_slug: preauth-instacash
scheme_count: 1
schemes:
- description: API token sent in the x-auth-token header on every request. Issued in the developer panel (https://dashboard.preauth.io/panel/devs). Test tokens carry a token_test_ prefix; production tokens are issued after a certification call.
  in: header
  name: apiToken
  parameter_name: x-auth-token
  sources:
  - openapi/preauth-instacash-orders-openapi.yml
  type: apiKey
slug: preauth-instacash-authentication
source_filename: preauth-instacash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.preauth.io/api-rest.md ; https://docs.preauth.io/primeros-pasos.md\ndocs: https://docs.preauth.io/api-rest.md#autenticacion\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter_name: x-auth-token\n    description: >-\n      API token sent in the x-auth-token header on every request. Issued in the\n      developer panel (https://dashboard.preauth.io/panel/devs). Test tokens carry a\n      token_test_ prefix; production tokens are issued after a certification call.\n    sources: [openapi/preauth-instacash-orders-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preauth-instacash/refs/heads/main/authentication/preauth-instacash-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Payment Pre-Authorization
- Payment Guarantees
- Fintech
- Latin America
- Cards
---
