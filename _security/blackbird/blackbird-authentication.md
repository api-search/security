---
api_key_in:
- header
api_specs:
- filename: blackbird-flynet-openapi-original.yml
  format: yaml
  label: Flynet API
  slug: flynet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-flynet-openapi-original.yml
auth_types:
- apiKey
- http
description: 'Flynet uses two credentials for two route families, never interchangeable: an X-API-Key (fly_live_/fly_test_) for Discovery routes (/restaurants*, /locations*, /check_ins feed), and an OAuth 2.0 + PKCE bearer JWT for member routes (/users/me/*) and all payment intent routes. The spec models the bearer as http/JWT; the OAuth flow and scopes are documented in scopes/blackbird-scopes.yml.'
kind: authentication
layout: security
method: searched
name: Blackbird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blackbird secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blackbird
provider_slug: blackbird
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 access token. Required for the `/users/me/*` routes

    (profile, status, wallets, tags, check-ins, memberships) and all

    payment intent routes.'
  name: oauthBearer
  scheme: bearer
  sources:
  - openapi/blackbird-flynet-openapi-original.yml
  type: http
- description: 'Server-to-server API key prefixed `fly_live_...` (production) or

    `fly_test_...` (staging/dev). Required on restaurant and location

    Discovery routes and on the `/check_ins` venue feed (key minted

    with `read:checkins`).'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/blackbird-flynet-openapi-original.yml
  type: apiKey
slug: blackbird-authentication
source_filename: blackbird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/blackbird-flynet-openapi-original.yml\ndocs: https://docs.flynet.org/concepts/authentication\ndescription: >-\n  Flynet uses two credentials for two route families, never interchangeable:\n  an X-API-Key (fly_live_/fly_test_) for Discovery routes (/restaurants*,\n  /locations*, /check_ins feed), and an OAuth 2.0 + PKCE bearer JWT for member\n  routes (/users/me/*) and all payment intent routes. The spec models the bearer\n  as http/JWT; the OAuth flow and scopes are documented in\n  scopes/blackbird-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth_variant: OAuth 2.0 + PKCE (Token-Mediating Backend)\nschemes:\n- name: oauthBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token. Required for the `/users/me/*` routes\n    (profile, status, wallets, tags, check-ins, memberships) and all\n    payment intent routes.\n  sources:\n\
  \  - openapi/blackbird-flynet-openapi-original.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    Server-to-server API key prefixed `fly_live_...` (production) or\n    `fly_test_...` (staging/dev). Required on restaurant and location\n    Discovery routes and on the `/check_ins` venue feed (key minted\n    with `read:checkins`).\n  sources:\n  - openapi/blackbird-flynet-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/authentication/blackbird-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Restaurants
- Loyalty
- Payments
- Dining
- Membership
- Crypto
- Blockchain
- Web3
---
