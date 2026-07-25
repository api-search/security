---
api_key_in: []
api_specs:
- filename: telr-agreements-api-openapi.yml
  format: yaml
  label: Telr Agreements API
  slug: telr-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-agreements-api-openapi.yml
- filename: telr-hosted-payment-page-api-openapi.yml
  format: yaml
  label: Telr Hosted Payment Page API
  slug: telr-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-hosted-payment-page-api-openapi.yml
- filename: telr-payments-api-api-openapi.yml
  format: yaml
  label: Telr Payments API API
  slug: telr-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-payments-api-api-openapi.yml
- filename: telr-remote-api-openapi.yml
  format: yaml
  label: Telr Remote API
  slug: telr-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-remote-api-openapi.yml
auth_types:
- http
- custom
description: ''
kind: authentication
layout: security
method: derived
name: Telr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telr secures its APIs with http and custom across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Telr
provider_slug: telr
scheme_count: 2
schemes:
- description: Legacy gateway endpoints (order.json, remote.json, manageagreement.json) authenticate with a numeric "store" id plus an "authkey" (authentication key) passed inside the JSON request body - not an HTTP header. The auth key is generated per store in Merchant Administration.
  in: body
  name: store_authkey
  parameters:
  - store
  - authkey
  sources:
  - openapi/telr-openapi.yml
  - https://docs.telr.com/reference/how-the-hosted-payment-page-works
  type: custom
- bearerFormat: null
  description: 'The REST Service / Payments / Accounts API (/api/v1/*) uses HTTP Basic authentication - username = store/merchant id, password = API key, Base64 encoded as "Authorization: Basic <base64(storeid:apikey)>". API keys are created in Merchant Administration under Integrations > Service API and can be scoped to specific services and restricted to publicly-routable IP addresses (comma-separated).'
  name: basic_auth
  scheme: basic
  sources:
  - https://docs.telr.com/reference/authentication
  - https://docs.telr.com/reference/api-configuration
  type: http
slug: telr-authentication
source_filename: telr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/telr-openapi.yml + https://docs.telr.com/reference/authentication + https://docs.telr.com/reference/api-configuration\nsummary:\n  types:\n  - http\n  - custom\nschemes:\n- name: store_authkey\n  type: custom\n  in: body\n  description: >-\n    Legacy gateway endpoints (order.json, remote.json, manageagreement.json)\n    authenticate with a numeric \"store\" id plus an \"authkey\" (authentication\n    key) passed inside the JSON request body - not an HTTP header. The auth key\n    is generated per store in Merchant Administration.\n  parameters:\n  - store\n  - authkey\n  sources:\n  - openapi/telr-openapi.yml\n  - https://docs.telr.com/reference/how-the-hosted-payment-page-works\n- name: basic_auth\n  type: http\n  scheme: basic\n  bearerFormat: null\n  description: >-\n    The REST Service / Payments / Accounts API (/api/v1/*) uses HTTP Basic\n    authentication - username = store/merchant id, password = API key, Base64\n\
  \    encoded as \"Authorization: Basic <base64(storeid:apikey)>\". API keys are\n    created in Merchant Administration under Integrations > Service API and can\n    be scoped to specific services and restricted to publicly-routable IP\n    addresses (comma-separated).\n  sources:\n  - https://docs.telr.com/reference/authentication\n  - https://docs.telr.com/reference/api-configuration\nnotes: >-\n  Two distinct auth styles coexist: in-body store+authkey for the classic\n  gateway JSON endpoints, and HTTP Basic (store id : API key) for the newer\n  REST /api/v1 surfaces. IP allow-listing is strongly recommended for Service\n  API keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/authentication/telr-authentication.yml
summary_line: http/custom · 2 schemes
tags:
- Payments
- Payment Gateway
- FinTech
- MENA
- UAE
---
