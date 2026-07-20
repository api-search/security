---
api_key_in: []
api_specs:
- filename: cabify-ride-hailing-openapi.yml
  format: yaml
  label: Cabify Ride-Hailing API
  slug: cabify-ride-hailing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-ride-hailing-openapi.yml
- filename: cabify-logistics-openapi.yml
  format: yaml
  label: Cabify Logistics API
  slug: cabify-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-logistics-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cabify Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cabify secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cabify
provider_slug: cabify
scheme_count: 2
schemes:
- name: access_token
  scheme: bearer
  sources:
  - openapi/cabify-ride-hailing-openapi.yml
  type: http
- name: bearer_token
  scheme: bearer
  sources:
  - openapi/cabify-logistics-openapi.yml
  type: http
slug: cabify-authentication
source_filename: cabify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.cabify.com/docs/get-your-access-token\ndocs: https://developers.cabify.com/docs/getting-started\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  http_schemes:\n  - bearer\nmodel: >-\n  Cabify uses OAuth2 client-credentials. Admin users generate an OAUTH_ID (client_id) and\n  CLIENT_SECRET from the Cabify Business admin panel (Integration section). Clients exchange these\n  for a short-lived Bearer access token, then send it on every request in the Authorization header.\n  The same credentials work for both the Ride-Hailing and Logistics APIs; production and sandbox are\n  independent environments with independent credentials.\ntoken_endpoint:\n  production: https://cabify.com/auth/api/authorization\n  sandbox: https://cabify-sandbox.com/auth/api/authorization\n  grant_type: client_credentials\n  request: 'POST grant_type=client_credentials&client_id=OAUTH_ID&client_secret=SECRET'\n\
  \  response_fields:\n  - token_type (Bearer)\n  - access_token\n  - expires_in (seconds; ~30 days)\ntoken_revocation:\n  method: DELETE\n  endpoint: /auth/api/authorization\n  header: 'Authorization: Bearer <token>'\n  success: 204\nrequest_header: 'Authorization: Bearer <access_token>'\nnotes: >-\n  Token refresh logic is client-side: create a new token before expires_in elapses. The underlying\n  OpenAPI securitySchemes are declared as http/bearer (access_token for Ride-Hailing, bearer_token\n  for Logistics); the client-credentials issuance flow is documented in the developer portal.\nschemes:\n- name: access_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cabify-ride-hailing-openapi.yml\n- name: bearer_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cabify-logistics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/authentication/cabify-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Transportation
- Ride Hailing
- Mobility
- Logistics
- Delivery
- Last Mile Delivery
- Webhooks
- OAuth
---
