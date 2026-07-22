---
api_key_in: []
api_specs:
- filename: nomos-openapi-original.json
  format: json
  label: Nomos API
  slug: nomos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-openapi-original.json
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
- OAuth
- Webhooks
---
