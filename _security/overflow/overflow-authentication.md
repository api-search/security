---
api_key_in:
- header
api_specs:
- filename: overflow-campaigns-api-openapi.yml
  format: yaml
  label: Overflow Campaigns API
  slug: overflow-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-campaigns-api-openapi.yml
- filename: overflow-chargebacks-api-openapi.yml
  format: yaml
  label: Overflow Chargebacks API
  slug: overflow-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-chargebacks-api-openapi.yml
- filename: overflow-contributions-api-openapi.yml
  format: yaml
  label: Overflow Contributions API
  slug: overflow-contributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-contributions-api-openapi.yml
- filename: overflow-deposits-api-openapi.yml
  format: yaml
  label: Overflow Deposits API
  slug: overflow-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-deposits-api-openapi.yml
- filename: overflow-donors-api-openapi.yml
  format: yaml
  label: Overflow Donors API
  slug: overflow-donors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-donors-api-openapi.yml
- filename: overflow-locations-api-openapi.yml
  format: yaml
  label: Overflow Locations API
  slug: overflow-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-locations-api-openapi.yml
- filename: overflow-payment-methods-api-openapi.yml
  format: yaml
  label: Overflow Payment Methods API
  slug: overflow-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-payment-methods-api-openapi.yml
- filename: overflow-payments-api-openapi.yml
  format: yaml
  label: Overflow Payments API
  slug: overflow-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-payments-api-openapi.yml
- filename: overflow-refunds-api-openapi.yml
  format: yaml
  label: Overflow Refunds API
  slug: overflow-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-refunds-api-openapi.yml
- filename: overflow-status-api-openapi.yml
  format: yaml
  label: Overflow Status API
  slug: overflow-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-status-api-openapi.yml
- filename: overflow-subscriptions-api-openapi.yml
  format: yaml
  label: Overflow Subscriptions API
  slug: overflow-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-subscriptions-api-openapi.yml
- filename: overflow-tap-api-openapi.yml
  format: yaml
  label: Overflow Tap API
  slug: overflow-tap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-tap-api-openapi.yml
- filename: overflow-webhooks-api-openapi.yml
  format: yaml
  label: Overflow Webhooks API
  slug: overflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Overflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overflow secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Overflow
provider_slug: overflow
scheme_count: 2
schemes:
- description: API Key for API authentication
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/overflow-openapi-original.json
  type: apiKey
- description: Client ID for API authentication
  in: header
  name: ClientId
  parameter: x-client-id
  sources:
  - openapi/overflow-openapi-original.json
  type: apiKey
slug: overflow-authentication
source_filename: overflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/overflow-openapi-original.json\ndocs: https://docs.overflow.co/api-reference/authentication\ndetail: >-\n  Overflow authenticates every request with two header-based API keys used\n  together: x-client-id (public identifier) and x-api-key (secret key).\n  Credentials are environment-scoped — staging credentials only work against\n  https://server.stage.overflow.co and production credentials only against\n  https://server.overflow.co. Credentials are server-side only and must not be\n  exposed in client-side code, public repos, or logs. There is no OAuth or\n  scope surface; access is all-or-nothing per credential pair.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key for API authentication\n  sources:\n  - openapi/overflow-openapi-original.json\n- name: ClientId\n  type: apiKey\n  in: header\n  parameter:\
  \ x-client-id\n  description: Client ID for API authentication\n  sources:\n  - openapi/overflow-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/authentication/overflow-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fintech
- Payments
- Donations
- Fundraising
- Non-Profit
- Giving
- Recurring Payments
- Webhook
- Cryptocurrency
---
