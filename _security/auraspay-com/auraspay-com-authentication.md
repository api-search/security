---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: auraspay-com-account-api-openapi.yml
  format: yaml
  label: AurasPay Account API
  slug: auraspay-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-account-api-openapi.yml
- filename: auraspay-com-agent-checkout-api-openapi.yml
  format: yaml
  label: AurasPay Agent Checkout API
  slug: auraspay-com-agent-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-agent-checkout-api-openapi.yml
- filename: auraspay-com-payment-links-api-openapi.yml
  format: yaml
  label: AurasPay Payment Links API
  slug: auraspay-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-payment-links-api-openapi.yml
- filename: auraspay-com-supported-tokens-api-openapi.yml
  format: yaml
  label: AurasPay Supported Tokens API
  slug: auraspay-com-supported-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-supported-tokens-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: AurasPay Authentication
name_suffix: Authentication
oauth_flows: []
overview: AurasPay secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AurasPay
provider_slug: auraspay-com
scheme_count: 2
schemes:
- description: Send the API key as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/auraspay-com-openapi.json
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/auraspay-com-openapi.json
  type: apiKey
slug: auraspay-com-authentication
source_filename: auraspay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/auraspay-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Send the API key as a Bearer token.\n  sources:\n  - openapi/auraspay-com-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/auraspay-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/auraspay-com/authentication/auraspay-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
---
