---
api_key_in:
- header
api_specs:
- filename: overflow-openapi-original.json
  format: json
  label: Overflow Open API
  slug: overflow-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-openapi-original.json
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
- Nonprofit
- Giving
- Recurring Payments
- Webhooks
- Cryptocurrency
---
