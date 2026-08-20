---
api_key_in: []
api_specs:
- filename: upbit-exchange-account-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Account API
  slug: upbit-exchange-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-account-api-openapi.yml
- filename: upbit-exchange-deposits-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Deposits API
  slug: upbit-exchange-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-deposits-api-openapi.yml
- filename: upbit-exchange-orders-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Orders API
  slug: upbit-exchange-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-orders-api-openapi.yml
- filename: upbit-exchange-service-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Service API
  slug: upbit-exchange-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-service-api-openapi.yml
- filename: upbit-exchange-travel-rule-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Travel Rule API
  slug: upbit-exchange-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-travel-rule-api-openapi.yml
- filename: upbit-exchange-withdrawals-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Withdrawals API
  slug: upbit-exchange-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-withdrawals-api-openapi.yml
- filename: upbit-quotation-api-openapi.yml
  format: yaml
  label: Upbit Quotation API
  slug: upbit-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-quotation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Upbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upbit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upbit
provider_slug: upbit
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT HS512 token generated from Access Key and Secret Key. Include query_hash and query_hash_alg=SHA512 in the payload when query parameters or JSON body exist.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: upbit-authentication
source_filename: upbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT HS512 token generated from Access Key and Secret Key. Include query_hash\n    and query_hash_alg=SHA512 in the payload when query parameters or JSON body exist.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/authentication/upbit-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Market Data
- Order
- Trading
- WebSocket
---
