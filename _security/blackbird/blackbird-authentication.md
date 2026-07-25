---
api_key_in:
- header
api_specs:
- filename: blackbird-app-api-openapi.yml
  format: yaml
  label: Blackbird App API
  slug: blackbird-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-app-api-openapi.yml
- filename: blackbird-challenges-api-openapi.yml
  format: yaml
  label: Blackbird Challenges API
  slug: blackbird-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-challenges-api-openapi.yml
- filename: blackbird-check-ins-api-openapi.yml
  format: yaml
  label: Blackbird Check-ins API
  slug: blackbird-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-check-ins-api-openapi.yml
- filename: blackbird-locations-api-openapi.yml
  format: yaml
  label: Blackbird Locations API
  slug: blackbird-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-locations-api-openapi.yml
- filename: blackbird-memberships-api-openapi.yml
  format: yaml
  label: Blackbird Memberships API
  slug: blackbird-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-memberships-api-openapi.yml
- filename: blackbird-payments-api-openapi.yml
  format: yaml
  label: Blackbird Payments API
  slug: blackbird-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-payments-api-openapi.yml
- filename: blackbird-restaurants-api-openapi.yml
  format: yaml
  label: Blackbird Restaurants API
  slug: blackbird-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-restaurants-api-openapi.yml
- filename: blackbird-rewards-api-openapi.yml
  format: yaml
  label: Blackbird Rewards API
  slug: blackbird-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-rewards-api-openapi.yml
- filename: blackbird-specials-api-openapi.yml
  format: yaml
  label: Blackbird Specials API
  slug: blackbird-specials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-specials-api-openapi.yml
- filename: blackbird-users-api-openapi.yml
  format: yaml
  label: Blackbird Users API
  slug: blackbird-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-users-api-openapi.yml
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
