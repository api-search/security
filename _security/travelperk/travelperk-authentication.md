---
api_key_in:
- header
api_specs:
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Bookings & Trips API
  slug: travelperk-bookings-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Invoices API
  slug: travelperk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Expenses API
  slug: travelperk-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Travelers & Members API
  slug: travelperk-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Cost Centers API
  slug: travelperk-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Webhooks API
  slug: travelperk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Travelperk Authentication
name_suffix: Authentication
oauth_flows: []
overview: TravelPerk secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TravelPerk
provider_slug: travelperk
scheme_count: 2
schemes:
- bearerFormat: token
  description: 'OAuth 2.0 access token obtained via the Authorization Code grant, passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/travelperk-openapi.yml
  type: http
- description: 'Personal API key passed as `Authorization: ApiKey <key>` for customer (non-partner) integrations.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/travelperk-openapi.yml
  type: apiKey
slug: travelperk-authentication
source_filename: travelperk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travelperk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: 'OAuth 2.0 access token obtained via the Authorization Code grant, passed as\n    `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/travelperk-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Personal API key passed as `Authorization: ApiKey <key>` for customer (non-partner)\n    integrations.'\n  sources:\n  - openapi/travelperk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/authentication/travelperk-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Business Travel
- Travel Management
- Expenses
- Invoices
- Bookings
---
