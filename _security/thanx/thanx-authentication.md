---
api_key_in:
- header
api_specs:
- filename: thanx-consumer-api-openapi.yml
  format: yaml
  label: Thanx Consumer API
  slug: consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-consumer-api-openapi.yml
- filename: thanx-partner-api-openapi.yml
  format: yaml
  label: Thanx Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-partner-api-openapi.yml
- filename: thanx-loyalty-api-openapi.yml
  format: yaml
  label: Thanx Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-loyalty-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thanx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thanx secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thanx
provider_slug: thanx
scheme_count: 3
schemes:
- description: End-user access token acquired through Thanx SSO.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thanx-consumer-api-openapi.yml
  - openapi/thanx-loyalty-api-openapi.yml
  - openapi/thanx-partner-api-openapi.yml
  type: http
- description: Client-specific identifier provided by Thanx.
  in: header
  name: clientId
  parameter: X-ClientId
  sources:
  - openapi/thanx-consumer-api-openapi.yml
  - openapi/thanx-partner-api-openapi.yml
  type: apiKey
- description: Merchant key provided by Thanx.
  in: header
  name: merchantKey
  parameter: Merchant-Key
  sources:
  - openapi/thanx-loyalty-api-openapi.yml
  type: apiKey
slug: thanx-authentication
source_filename: thanx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thanx-consumer-api-openapi.yml, openapi/thanx-loyalty-api-openapi.yml, openapi/thanx-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: End-user access token acquired through Thanx SSO.\n  sources:\n  - openapi/thanx-consumer-api-openapi.yml\n  - openapi/thanx-loyalty-api-openapi.yml\n  - openapi/thanx-partner-api-openapi.yml\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-ClientId\n  description: Client-specific identifier provided by Thanx.\n  sources:\n  - openapi/thanx-consumer-api-openapi.yml\n  - openapi/thanx-partner-api-openapi.yml\n- name: merchantKey\n  type: apiKey\n  in: header\n  parameter: Merchant-Key\n  description: Merchant key provided by Thanx.\n  sources:\n  - openapi/thanx-loyalty-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/authentication/thanx-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhooks
- Points
- Rewards
- Campaigns
---
