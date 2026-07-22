---
api_key_in: []
api_specs:
- filename: noyo-fulfillment-openapi.json
  format: json
  label: Noyo Fulfillment API
  slug: noyo-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-fulfillment-openapi.json
- filename: noyo-tracking-openapi.json
  format: json
  label: Noyo Tracking API
  slug: noyo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-tracking-openapi.json
- filename: noyo-carrier-openapi.json
  format: json
  label: Noyo Carrier API
  slug: noyo-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-carrier-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Noyo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Noyo secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Noyo
provider_slug: noyo
scheme_count: 2
schemes:
- client_auth: basic
  flow: clientCredentials
  grant_type: client_credentials
  name: clientCredentials
  sources:
  - docs
  token_ttl_seconds: 600
  token_type: Bearer
  token_url: https://accounts.noyo.com/auth/public/token
  type: oauth2
- description: 'Short-lived access token returned by the token endpoint, sent as: Authorization Bearer <ACCESS_TOKEN>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
slug: noyo-authentication
source_filename: noyo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.noyo.com/docs/introduction/getting-started/authentication\ndocs: https://docs.noyo.com/docs/introduction/getting-started/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\n  notes: >-\n    Noyo issues API keys (CLIENT_ID / CLIENT_SECRET) managed by an organization\n    admin in the Noyo web application. Keys are exchanged for a short-lived\n    bearer access token via an OAuth2 client-credentials style token endpoint;\n    the CLIENT_ID:CLIENT_SECRET pair is sent as HTTP Basic auth on the token\n    request. The returned access_token is then sent as a Bearer token on each\n    API call. Sandbox and production use separate keys. The OpenAPI documents\n    do not declare securitySchemes, so this profile is sourced from the docs.\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://accounts.noyo.com/auth/public/token\n\
  \  grant_type: client_credentials\n  client_auth: basic\n  token_type: Bearer\n  token_ttl_seconds: 600\n  sources: [docs]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Short-lived access token returned by the token endpoint, sent as: Authorization Bearer <ACCESS_TOKEN>.'\n  sources: [docs]\nenvironments:\n  production: https://fulfillment.noyo.com\n  sandbox: https://fulfillment-sandbox.noyo.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/authentication/noyo-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Insurance
- Employee Benefits
- Enrollment
- Benefits Administration
- Insurance Carriers
- Data Exchange
- Webhooks
- Health Insurance
---
