---
api_key_in: []
api_specs:
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay COPYandPAY API
  slug: hyperpay-copyandpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Server-to-Server Payments API
  slug: hyperpay-server-to-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Registration Tokens API
  slug: hyperpay-registration-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Query API
  slug: hyperpay-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hyperpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: HyperPay secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HyperPay
provider_slug: hyperpay
scheme_count: 2
schemes:
- bearerFormat: accessToken
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/hyperpay-openapi.yml
  type: http
- in: query
  name: entity_id
  note: Also sent as a form field on POST requests; identifies the merchant channel.
  paramName: entityId
  sources:
  - openapi/hyperpay-openapi.yml
  type: apiKey
slug: hyperpay-authentication
source_filename: hyperpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/hyperpay-openapi.yml\ndocs: https://hyperpay.docs.oppwa.com/reference/parameters\nsummary:\n  types:\n  - http\nnotes: >-\n  HyperPay (ACI / OPPWA) authenticates every request with TWO credentials issued\n  together: an `entityId` channel identifier (a form field on writes, a query\n  parameter on reads) that scopes the request to a specific merchant channel, and\n  an `Authorization: Bearer <access-token>` header. Requests are\n  application/x-www-form-urlencoded over TLS. Separate entityId values are issued\n  per payment-method channel (e.g. one for cards, one for mada, one for Apple\n  Pay). Test and live use distinct credentials and hosts.\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: accessToken\n  sources:\n  - openapi/hyperpay-openapi.yml\n- name: entity_id\n  type: apiKey\n  in: query\n  paramName: entityId\n  note: Also sent as a form field on POST requests; identifies the\
  \ merchant channel.\n  sources:\n  - openapi/hyperpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/authentication/hyperpay-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- mada
- Apple Pay
- Cards
---
