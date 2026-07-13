---
api_key_in: []
api_specs:
- filename: affirm-checkout-openapi.yml
  format: yaml
  label: Affirm Checkout API
  slug: affirm-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-checkout-openapi.yml
- filename: affirm-transactions-openapi.yml
  format: yaml
  label: Affirm Transactions API
  slug: affirm-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transactions-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Affirm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affirm secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affirm
provider_slug: affirm
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using the merchant's public API key as the username and private API key as the password, Base64-encoded as per RFC 7617.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/affirm-checkout-openapi.yml
  - openapi/affirm-direct-api-openapi.yml
  - openapi/affirm-disputes-openapi.yml
  - openapi/affirm-transactions-openapi.yml
  type: http
slug: affirm-authentication
source_filename: affirm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/affirm-checkout-openapi.yml, openapi/affirm-direct-api-openapi.yml, openapi/affirm-disputes-openapi.yml,\n  openapi/affirm-transactions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using the merchant's public API key as the username\n    and private API key as the password, Base64-encoded as per RFC 7617.\n  sources:\n  - openapi/affirm-checkout-openapi.yml\n  - openapi/affirm-direct-api-openapi.yml\n  - openapi/affirm-disputes-openapi.yml\n  - openapi/affirm-transactions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/authentication/affirm-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- BNPL
- Lending
- Payments
- Consumer
---
