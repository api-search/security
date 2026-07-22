---
api_key_in:
- header
api_specs:
- filename: weavr-multi-openapi-original.yml
  format: yaml
  label: Weavr Multi Product API
  slug: weavr-multi-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-multi-openapi-original.yml
- filename: weavr-multi-backoffice-openapi-original.yml
  format: yaml
  label: Weavr Multi Product BackOffice API
  slug: weavr-multi-product-backoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-multi-backoffice-openapi-original.yml
- filename: weavr-payment-run-openapi-original.yml
  format: yaml
  label: Weavr Embedded Payment Run API
  slug: weavr-embedded-payment-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-payment-run-openapi-original.yml
- filename: weavr-simulator-openapi-original.yml
  format: yaml
  label: Weavr Simulator
  slug: weavr-simulator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-simulator-openapi-original.yml
- filename: weavr-webhooks-openapi-original.yml
  format: yaml
  label: Weavr Webhook
  slug: weavr-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-webhooks-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Weavr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weavr secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Weavr
provider_slug: weavr
scheme_count: 4
schemes:
- description: The API Key representing your Multi account.
  in: header
  name: api_key
  parameter: api-key
  sources:
  - openapi/weavr-multi-backoffice-openapi-original.yml
  - openapi/weavr-multi-openapi-original.yml
  - openapi/weavr-payment-run-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: The authentication token representing the user. This will be included in the login response object.
  name: auth_token
  scheme: bearer
  sources:
  - openapi/weavr-multi-backoffice-openapi-original.yml
  - openapi/weavr-multi-openapi-original.yml
  - openapi/weavr-payment-run-openapi-original.yml
  - openapi/weavr-simulator-openapi-original.yml
  type: http
- description: The Webhooks key can be found in the API Credentials tab in your Portal Page.
  in: header
  name: webhooks_key
  parameter: webhooks-key
  sources:
  - openapi/weavr-multi-openapi-original.yml
  type: apiKey
- description: The API Secret Key - available from the Configuration area of the Innovator Portal
  in: header
  name: API_Secret_Key
  parameter: programme-key
  sources:
  - openapi/weavr-simulator-openapi-original.yml
  type: apiKey
slug: weavr-authentication
source_filename: weavr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/weavr-multi-backoffice-openapi-original.yml, openapi/weavr-multi-openapi-original.yml,\n  openapi/weavr-payment-run-openapi-original.yml, openapi/weavr-simulator-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: The API Key representing your Multi account.\n  sources:\n  - openapi/weavr-multi-backoffice-openapi-original.yml\n  - openapi/weavr-multi-openapi-original.yml\n  - openapi/weavr-payment-run-openapi-original.yml\n- name: auth_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: The authentication token representing the user. This will be included in the\n    login response object.\n  sources:\n  - openapi/weavr-multi-backoffice-openapi-original.yml\n  - openapi/weavr-multi-openapi-original.yml\n  - openapi/weavr-payment-run-openapi-original.yml\n  - openapi/weavr-simulator-openapi-original.yml\n\
  - name: webhooks_key\n  type: apiKey\n  in: header\n  parameter: webhooks-key\n  description: The Webhooks key can be found in the API Credentials tab in your Portal Page.\n  sources:\n  - openapi/weavr-multi-openapi-original.yml\n- name: API_Secret_Key\n  type: apiKey\n  in: header\n  parameter: programme-key\n  description: The API Secret Key - available from the Configuration area of the Innovator Portal\n  sources:\n  - openapi/weavr-simulator-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/authentication/weavr-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Embedded Finance
- Banking as a Service
- Payments
- Cards
- Fintech
- Accounts
- KYC
- Company
---
