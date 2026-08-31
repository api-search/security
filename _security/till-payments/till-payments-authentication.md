---
api_key_in:
- path
api_specs:
- filename: till-payments-continue-dcc-api-openapi.yml
  format: yaml
  label: Till Payments Continue Dcc API
  slug: till-payments-continue-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-continue-dcc-api-openapi.yml
- filename: till-payments-dispute-api-openapi.yml
  format: yaml
  label: Till Payments Dispute API
  slug: till-payments-dispute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-dispute-api-openapi.yml
- filename: till-payments-options-api-openapi.yml
  format: yaml
  label: Till Payments Options API
  slug: till-payments-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-options-api-openapi.yml
- filename: till-payments-prepare-transaction-api-openapi.yml
  format: yaml
  label: Till Payments Prepare Transaction API
  slug: till-payments-prepare-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-prepare-transaction-api-openapi.yml
- filename: till-payments-schedule-api-openapi.yml
  format: yaml
  label: Till Payments Schedule API
  slug: till-payments-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-schedule-api-openapi.yml
- filename: till-payments-status-api-openapi.yml
  format: yaml
  label: Till Payments Status API
  slug: till-payments-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-status-api-openapi.yml
- filename: till-payments-transaction-api-openapi.yml
  format: yaml
  label: Till Payments Transaction API
  slug: till-payments-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-transaction-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Till Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Till Payments secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Till Payments
provider_slug: till-payments
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/till-payments-direct-pci.yml
  - openapi/till-payments-gateway.yml
  type: http
- description: Per-connector API key embedded as a path segment on every transaction endpoint.
  in: path
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/till-payments-gateway.yml
  - openapi/till-payments-direct-pci.yml
  type: apiKey
- algorithm: HMAC-SHA512
  description: 'Optional, connector-enabled request signing ("API: Enable Request Signing"). Recommended for production integrations to verify request integrity.'
  encoding: base64
  name: requestSignature
  required: false
  source: https://gateway.tillpayments.com/documentation/apiv3
  type: signature
slug: till-payments-authentication
source_filename: till-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/till-payments-direct-pci.yml, openapi/till-payments-gateway.yml\ndocs: https://gateway.tillpayments.com/documentation/apiv3\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in:\n  - path\n  request_signing: optional\nnotes: >-\n  Every Till Payments Gateway and Direct PCI request authenticates with HTTP\n  Basic credentials over TLS 1.2+. The API username and password are joined by a\n  colon and Base64-encoded into the Authorization: Basic header (docs example:\n  anyApiUser:myPassword -> Authorization: Basic YW55QXBpVXNlcjpteVBhc3N3b3Jk). In\n  addition, every transaction endpoint carries a per-connector apiKey as a path\n  parameter (/api/v3/transaction/{apiKey}/debit). Request signing is optionally\n  available and recommended: an HMAC-SHA512 signature (Base64) enabled per\n  connector via the \"API: Enable Request Signing\" setting. No OAuth2/OIDC surface\n  is exposed, so there is no scope\
  \ model.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/till-payments-direct-pci.yml\n  - openapi/till-payments-gateway.yml\n- name: apiKey\n  type: apiKey\n  in: path\n  parameter: apiKey\n  description: Per-connector API key embedded as a path segment on every transaction endpoint.\n  sources:\n  - openapi/till-payments-gateway.yml\n  - openapi/till-payments-direct-pci.yml\n- name: requestSignature\n  type: signature\n  algorithm: HMAC-SHA512\n  encoding: base64\n  required: false\n  description: >-\n    Optional, connector-enabled request signing (\"API: Enable Request Signing\").\n    Recommended for production integrations to verify request integrity.\n  source: https://gateway.tillpayments.com/documentation/apiv3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/authentication/till-payments-authentication.yml
summary_line: http · 3 schemes
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- Card Payments
- In-Person Payments
---
