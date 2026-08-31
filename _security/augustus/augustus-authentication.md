---
api_key_in:
- header
api_specs:
- filename: augustus-account-programs-api-openapi.yml
  format: yaml
  label: Augustus Account Programs API
  slug: augustus-account-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-account-programs-api-openapi.yml
- filename: augustus-accounts-api-openapi.yml
  format: yaml
  label: Augustus Accounts API
  slug: augustus-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-accounts-api-openapi.yml
- filename: augustus-api-key-api-openapi.yml
  format: yaml
  label: Augustus API Key API
  slug: augustus-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-api-key-api-openapi.yml
- filename: augustus-api-versions-api-openapi.yml
  format: yaml
  label: Augustus API Versions API
  slug: augustus-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-api-versions-api-openapi.yml
- filename: augustus-conversions-api-openapi.yml
  format: yaml
  label: Augustus Conversions API
  slug: augustus-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-conversions-api-openapi.yml
- filename: augustus-deposits-api-openapi.yml
  format: yaml
  label: Augustus Deposits API
  slug: augustus-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-deposits-api-openapi.yml
- filename: augustus-events-api-openapi.yml
  format: yaml
  label: Augustus Events API
  slug: augustus-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-events-api-openapi.yml
- filename: augustus-payouts-api-openapi.yml
  format: yaml
  label: Augustus Payouts API
  slug: augustus-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-payouts-api-openapi.yml
- filename: augustus-quotes-api-openapi.yml
  format: yaml
  label: Augustus Quotes API
  slug: augustus-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-quotes-api-openapi.yml
- filename: augustus-returns-api-openapi.yml
  format: yaml
  label: Augustus Returns API
  slug: augustus-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-returns-api-openapi.yml
- filename: augustus-scopes-api-openapi.yml
  format: yaml
  label: Augustus Scopes API
  slug: augustus-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-scopes-api-openapi.yml
- filename: augustus-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Augustus Webhook Deliveries API
  slug: augustus-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-webhook-deliveries-api-openapi.yml
- filename: augustus-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Augustus Webhook Subscriptions API
  slug: augustus-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-webhook-subscriptions-api-openapi.yml
- filename: augustus-webhook-events-api-openapi.yml
  format: yaml
  label: Augustus Webhook Events API
  slug: augustus-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-webhook-events-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Augustus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Augustus secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Augustus
provider_slug: augustus
scheme_count: 2
schemes:
- api: Augustus Banking API (2026-05-01)
  bearerFormat: JWT
  description: The 2026-05-01 Augustus Banking API authenticates with a bearer token in the standard Authorization header. Keys are environment-prefixed (e.g. sandbox., prod.) and otherwise opaque. Each key carries one or more scopes.
  header: 'Authorization: Bearer {api_key}'
  key_prefixes:
  - sandbox.
  - prod.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/augustus-openapi-original.yml
  type: http
- api: Ivy API (2023-01-01)
  description: The legacy Ivy Open Banking API authenticates with the X-Ivy-Api-Key header. Existing Ivy customers keep using their keys unchanged. Keys are managed and rotated in the Augustus Dashboard.
  in: header
  name: IvyApiKey
  parameter: X-Ivy-Api-Key
  sources:
  - https://docs.augustus.com/reference/authentication
  type: apiKey
slug: augustus-authentication
source_filename: augustus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/augustus-openapi-original.yml\ndocs:\n- https://docs.augustus.com/v1/authentication\n- https://docs.augustus.com/reference/authentication\n- https://docs.augustus.com/v1/scopes\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Augustus uses scoped bearer API keys. Two API generations authenticate\n    differently. All requests must be over HTTPS; plain HTTP or unauthenticated\n    requests fail. Keys can optionally be restricted to IP addresses / CIDR\n    ranges (IPv4 + IPv6) at creation time.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  api: Augustus Banking API (2026-05-01)\n  header: 'Authorization: Bearer {api_key}'\n  description: >-\n    The 2026-05-01 Augustus Banking API authenticates with a bearer token in the\n    standard Authorization header. Keys are environment-prefixed (e.g. sandbox.,\n    prod.) and otherwise\
  \ opaque. Each key carries one or more scopes.\n  key_prefixes:\n  - sandbox.\n  - prod.\n  sources:\n  - openapi/augustus-openapi-original.yml\n- name: IvyApiKey\n  type: apiKey\n  in: header\n  parameter: X-Ivy-Api-Key\n  api: Ivy API (2023-01-01)\n  description: >-\n    The legacy Ivy Open Banking API authenticates with the X-Ivy-Api-Key header.\n    Existing Ivy customers keep using their keys unchanged. Keys are managed and\n    rotated in the Augustus Dashboard.\n  sources:\n  - https://docs.augustus.com/reference/authentication\nscopes_model:\n  shape: 'resource:action'\n  actions:\n  - read\n  - write\n  enforcement: Every request; a 403 insufficient_scope carries a required_scopes array.\n  catalogue_endpoint: GET /v1/scopes\n  reference: scopes/augustus-scopes.yml\nerrors:\n- status: 401\n  code: authentication_required\n  when: Missing or invalid API key\n- status: 403\n  code: permission_denied\n  when: Valid key but insufficient permissions (non-scope check)\n- status: 403\n\
  \  code: insufficient_scope\n  when: Valid key missing one or more required scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/authentication/augustus-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Stablecoins
- Payouts
- Foreign Exchange
- Webhook
---
