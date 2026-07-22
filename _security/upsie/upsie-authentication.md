---
api_key_in:
- header
api_specs:
- filename: upsie-partner-network-openapi.yml
  format: yaml
  label: Upsie Partner Network API
  slug: upsie-partner-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upsie/refs/heads/main/openapi/upsie-partner-network-openapi.yml
auth_types:
- apiKey
description: Authentication profile for the Upsie Partner Network API, captured from the official Postman documentation (api.upsie.com/docs). The API authenticates every request with a JSON Web Token passed in a custom `token` header. Tokens are obtained by partner-user login (username/password) and then exchanged for longer-lived API access and refresh tokens; partner-scoped API access tokens can also be generated and invalidated through the Upsie Partner Portal.
kind: authentication
layout: security
method: searched
name: Upsie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upsie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upsie
provider_slug: upsie
scheme_count: 1
schemes:
- format: JWT
  in: header
  name: jwtToken
  notes: 'JWT passed in a `token` header with each API request. Documented token lifetimes: access tokens 30 days, refresh tokens 60 days, partner-scoped API access tokens 10 years. Tokens carry an encoded expiration date and can be invalidated at any time via POST /partner/auth/invalidateapitokens or the Partner Portal.'
  parameter: token
  sources:
  - openapi/upsie-partner-network-openapi.yml
  type: apiKey
slug: upsie-authentication
source_filename: upsie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://documenter.getpostman.com/view/16328390/2s8ZDeUykK\ndescription: >-\n  Authentication profile for the Upsie Partner Network API, captured from the\n  official Postman documentation (api.upsie.com/docs). The API authenticates\n  every request with a JSON Web Token passed in a custom `token` header. Tokens\n  are obtained by partner-user login (username/password) and then exchanged for\n  longer-lived API access and refresh tokens; partner-scoped API access tokens\n  can also be generated and invalidated through the Upsie Partner Portal.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  header_name: token\n  token_format: JWT\nschemes:\n  - name: jwtToken\n    type: apiKey\n    in: header\n    parameter: token\n    format: JWT\n    sources: [openapi/upsie-partner-network-openapi.yml]\n    notes: >-\n      JWT passed in a `token` header with each API request. Documented token\n      lifetimes: access tokens 30 days,\
  \ refresh tokens 60 days, partner-scoped\n      API access tokens 10 years. Tokens carry an encoded expiration date and\n      can be invalidated at any time via POST /partner/auth/invalidateapitokens\n      or the Partner Portal.\nflows:\n  - step: 1\n    operation: partnerLogin\n    request: POST /partner/auth/login\n    detail: Partner user login with username/password returns a user JWT.\n  - step: 2\n    operation: generateApiAccessToken\n    request: POST /partner/auth/apiaccess\n    detail: Exchange the user token for an API access token (30-day expiry).\n  - step: 3\n    operation: generateApiRefreshToken\n    request: POST /partner/auth/apirefresh\n    detail: Refresh tokens (60-day expiry) mint new access tokens.\n  - step: 4\n    operation: whoAmI\n    request: GET /partner/auth/whoami\n    detail: Verify the identity bound to the presented token.\n  - step: 5\n    operation: invalidateApiTokens\n    request: POST /partner/auth/invalidateapitokens\n    detail: Invalidate the\
  \ account's API tokens if lost or stolen.\nguidance:\n  - Do not share API keys in publicly accessible areas such as GitHub or client-side code.\n  - Always use HTTPS when making API requests.\n  - Invalidate tokens immediately if one is suspected lost or stolen.\ncontact: dev@upsie.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsie/refs/heads/main/authentication/upsie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Warranties
- Protection Plans
- Consumer Electronics
- Repairs
- Insurance
---
