---
api_key_in:
- header
api_specs:
- filename: thefork-b2b-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-b2b-openapi.yml
- filename: thefork-pos-openapi.yml
  format: yaml
  label: TheFork POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-pos-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Thefork Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TheFork secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TheFork
provider_slug: thefork
scheme_count: 3
schemes:
- description: Auth0 OAuth 2.0 client credentials flow. Exchange client_id and client_secret for a bearer token at https://auth.thefork.io/oauth/token with audience https://api.thefork.io. Tokens expire after 8600 seconds.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.thefork.io/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/thefork-b2b-openapi.yml
  type: oauth2
- description: API key issued by TheFork for POS API v1.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/thefork-pos-openapi.yml
  type: apiKey
- description: Bearer token presented by TheFork on calls to the POS provider.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/thefork-pos-openapi.yml
  type: http
slug: thefork-authentication
source_filename: thefork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thefork-b2b-openapi.yml, openapi/thefork-pos-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.thefork.io/oauth/token\n    scopes: 0\n  description: Auth0 OAuth 2.0 client credentials flow. Exchange client_id and client_secret\n    for a bearer token at https://auth.thefork.io/oauth/token with audience https://api.thefork.io.\n    Tokens expire after 8600 seconds.\n  sources:\n  - openapi/thefork-b2b-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key issued by TheFork for POS API v1.\n  sources:\n  - openapi/thefork-pos-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: Bearer token presented by TheFork on calls to the POS provider.\n\
  \  sources:\n  - openapi/thefork-pos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/authentication/thefork-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Restaurant
- Reservations
- Booking
- Dining
- Point Of Sale
- Marketplace
---
