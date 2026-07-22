---
api_key_in:
- header
api_specs:
- filename: solvimon-configuration-api-openapi.yml
  format: yaml
  label: Solvimon Configuration API
  slug: solvimon-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-configuration-api-openapi.yml
- filename: solvimon-transaction-api-openapi.yml
  format: yaml
  label: Solvimon Transaction API
  slug: solvimon-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-transaction-api-openapi.yml
- filename: solvimon-identity-api-openapi.yml
  format: yaml
  label: Solvimon Identity API
  slug: solvimon-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-identity-api-openapi.yml
- filename: solvimon-event-api-openapi.yml
  format: yaml
  label: Solvimon Event API
  slug: solvimon-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-event-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Solvimon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solvimon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Solvimon
provider_slug: solvimon
scheme_count: 2
schemes:
- in: header
  name: API-Key
  parameter: X-API-KEY
  sources:
  - openapi/solvimon-configuration-api-openapi.yml
  - openapi/solvimon-event-api-openapi.yml
  - openapi/solvimon-identity-api-openapi.yml
  - openapi/solvimon-transaction-api-openapi.yml
  type: apiKey
- name: JWT-Authentication
  scheme: bearer
  sources:
  - openapi/solvimon-configuration-api-openapi.yml
  - openapi/solvimon-event-api-openapi.yml
  - openapi/solvimon-identity-api-openapi.yml
  - openapi/solvimon-transaction-api-openapi.yml
  token_endpoints:
  - /v1/oauth/token
  - /v1/oauth/refresh-token
  - /v1/oauth/sandbox-token
  - /v1/oauth/demo-token
  type: http
slug: solvimon-authentication
source_filename: solvimon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/solvimon-configuration-api-openapi.yml, openapi/solvimon-event-api-openapi.yml,\n  openapi/solvimon-identity-api-openapi.yml, openapi/solvimon-transaction-api-openapi.yml\ndocs: https://docs.solvimon.com/api-docs/solvimon-api/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  primary: api-key-header\n  notes: >-\n    Primary auth is a secret API key in the X-API-KEY header, issued per account\n    from Desk (Settings -> API keys), with distinct test and live keys. A JWT\n    bearer scheme (JWT-Authentication) is also defined across all four services;\n    the Identity API mints and refreshes tokens via /v1/oauth/token,\n    /v1/oauth/refresh-token, /v1/oauth/sandbox-token and /v1/oauth/demo-token.\n    Frontend SDK sessions use a short-lived portal-object token so the secret key\n    never reaches the browser. No OAuth2 scope scheme or OIDC discovery is\n    published.\nschemes:\n\
  - name: API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/solvimon-configuration-api-openapi.yml\n  - openapi/solvimon-event-api-openapi.yml\n  - openapi/solvimon-identity-api-openapi.yml\n  - openapi/solvimon-transaction-api-openapi.yml\n- name: JWT-Authentication\n  type: http\n  scheme: bearer\n  token_endpoints:\n  - /v1/oauth/token\n  - /v1/oauth/refresh-token\n  - /v1/oauth/sandbox-token\n  - /v1/oauth/demo-token\n  sources:\n  - openapi/solvimon-configuration-api-openapi.yml\n  - openapi/solvimon-event-api-openapi.yml\n  - openapi/solvimon-identity-api-openapi.yml\n  - openapi/solvimon-transaction-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/authentication/solvimon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Billing
- Payments
- Monetization
- Usage-Based Pricing
- Subscriptions
- Invoicing
- Metering
- Revenue Recognition
---
