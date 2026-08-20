---
api_key_in: []
api_specs:
- filename: nomos-authentication-api-openapi.yml
  format: yaml
  label: Nomos Authentication API
  slug: nomos-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-authentication-api-openapi.yml
- filename: nomos-customers-api-openapi.yml
  format: yaml
  label: Nomos Customers API
  slug: nomos-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-customers-api-openapi.yml
- filename: nomos-events-api-openapi.yml
  format: yaml
  label: Nomos Events API
  slug: nomos-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-events-api-openapi.yml
- filename: nomos-grid-fee-reductions-api-openapi.yml
  format: yaml
  label: Nomos Grid Fee Reductions API
  slug: nomos-grid-fee-reductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-grid-fee-reductions-api-openapi.yml
- filename: nomos-invoices-api-openapi.yml
  format: yaml
  label: Nomos Invoices API
  slug: nomos-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-invoices-api-openapi.yml
- filename: nomos-leads-api-openapi.yml
  format: yaml
  label: Nomos Leads API
  slug: nomos-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-leads-api-openapi.yml
- filename: nomos-market-partners-api-openapi.yml
  format: yaml
  label: Nomos Market Partners API
  slug: nomos-market-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-market-partners-api-openapi.yml
- filename: nomos-plans-api-openapi.yml
  format: yaml
  label: Nomos Plans API
  slug: nomos-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-plans-api-openapi.yml
- filename: nomos-prices-api-openapi.yml
  format: yaml
  label: Nomos Prices API
  slug: nomos-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-prices-api-openapi.yml
- filename: nomos-smart-meter-orders-api-openapi.yml
  format: yaml
  label: Nomos Smart Meter Orders API
  slug: nomos-smart-meter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-smart-meter-orders-api-openapi.yml
- filename: nomos-subscriptions-api-openapi.yml
  format: yaml
  label: Nomos Subscriptions API
  slug: nomos-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-subscriptions-api-openapi.yml
- filename: nomos-usage-api-openapi.yml
  format: yaml
  label: Nomos Usage API
  slug: nomos-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-usage-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nomos Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Nomos secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Nomos
provider_slug: nomos
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: Bearer
  note: JWT access token obtained via the OAuth 2.0 token endpoint.
  scheme: bearer
  sources:
  - openapi/nomos-openapi-original.json
  type: http
- name: Basic
  note: HTTP Basic used at /oauth/token to present client_id:client_secret (client_secret_basic).
  scheme: basic
  sources:
  - openapi/nomos-openapi-original.json
  type: http
slug: nomos-authentication
source_filename: nomos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nomos.energy/api-references/authentication\ndocs: https://docs.nomos.energy/api-references/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  model: >-\n    OAuth 2.0. Exchange client_id/client_secret for a short-lived JWT bearer\n    access token, then send Authorization: Bearer <token>. Client credentials\n    grant for server-to-server against your own org data; authorization code +\n    PKCE when acting on behalf of an end customer. HTTPS only.\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  token_ttl_seconds: 3600\n  scopes:\n  - 'read:*'\n  - 'write:*'\noauth2:\n  authorization_endpoint: https://api.nomos.energy/oauth/authorize\n  token_endpoint: https://api.nomos.energy/oauth/token\n  metadata: https://api.nomos.energy/.well-known/oauth-authorization-server\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  pkce: [S256, plain]\n  token_endpoint_auth_methods:\
  \ [client_secret_basic]\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: 'JWT access token obtained via the OAuth 2.0 token endpoint.'\n  sources:\n  - openapi/nomos-openapi-original.json\n- name: Basic\n  type: http\n  scheme: basic\n  note: 'HTTP Basic used at /oauth/token to present client_id:client_secret (client_secret_basic).'\n  sources:\n  - openapi/nomos-openapi-original.json\nsee:\n  scopes: scopes/nomos-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/authentication/nomos-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Energy
- Electricity
- Utilities
- Embedded Finance
- Dynamic Pricing
- Billing
- Metering
- Smart Meter
- Germany
- Authentication
- Webhook
---
