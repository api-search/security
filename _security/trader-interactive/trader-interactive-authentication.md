---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Trader Interactive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trader Interactive declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Trader Interactive
provider_slug: trader-interactive
scheme_count: 3
schemes:
- default: true
  evidence: 'tol-api-php Authentication::createClientCredentials() posts {client_id, client_secret, grant_type: client_credentials} to "{baseUrl}/{tokenResource}" where tokenResource defaults to "token"; tol-api-nodejs createClient() wires getClientCredentialsToken(apiUrl + ''/token'', clientId, clientSecret).'
  flow: clientCredentials
  id: oauth2_client_credentials
  parameters:
  - client_id
  - client_secret
  - grant_type=client_credentials
  token_url: '{baseUrl}/token'
  type: oauth2
- default: false
  evidence: tol-api-php Authentication::createResourceOwnerPasswordCredentials() and tol-api-nodejs getResourceOwnerPasswordCredentialsToken().
  flow: password
  id: oauth2_password
  parameters:
  - client_id
  - client_secret
  - username
  - password
  - grant_type=password
  token_url: '{baseUrl}/token'
  type: oauth2
- default: false
  evidence: Both clients implement refresh-token exchange. The PHP client exposes refreshResource separately from tokenResource with the comment "Only needed since apigee doesnt use the token resource that is in the oauth2 spec", indicating the TOL API is (or was) fronted by Apigee with a non-standard refresh endpoint.
  flow: refreshToken
  id: oauth2_refresh_token
  token_url: '{baseUrl}/{refreshResource}'
  type: oauth2
slug: trader-interactive-authentication
source_filename: trader-interactive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: >-\n  https://github.com/traderinteractive/tol-api-php/blob/master/src/Authentication.php,\n  https://github.com/traderinteractive/tol-api-php/blob/master/README.md,\n  https://github.com/traderinteractive/tol-api-nodejs/blob/master/index.js\nnote: >-\n  Trader Interactive publishes no authentication documentation. This profile is derived from the source\n  of the two first-party TOL API clients the company maintains, which is the only public description of\n  how the TraderOnline API authenticates. It is not a substitute for a published auth reference.\napi: TraderOnline (TOL) API\nbase_url: https://api.traderonline.com\nprimary_scheme: oauth2\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: '{baseUrl}/token'\n    parameters:\n      - client_id\n      - client_secret\n      - grant_type=client_credentials\n    default: true\n    evidence: >-\n      tol-api-php Authentication::createClientCredentials()\
  \ posts\n      {client_id, client_secret, grant_type: client_credentials} to \"{baseUrl}/{tokenResource}\" where\n      tokenResource defaults to \"token\"; tol-api-nodejs createClient() wires\n      getClientCredentialsToken(apiUrl + '/token', clientId, clientSecret).\n  - id: oauth2_password\n    type: oauth2\n    flow: password\n    token_url: '{baseUrl}/token'\n    parameters:\n      - client_id\n      - client_secret\n      - username\n      - password\n      - grant_type=password\n    default: false\n    evidence: >-\n      tol-api-php Authentication::createResourceOwnerPasswordCredentials() and\n      tol-api-nodejs getResourceOwnerPasswordCredentialsToken().\n  - id: oauth2_refresh_token\n    type: oauth2\n    flow: refreshToken\n    token_url: '{baseUrl}/{refreshResource}'\n    default: false\n    evidence: >-\n      Both clients implement refresh-token exchange. The PHP client exposes refreshResource separately\n      from tokenResource with the comment \"Only needed since apigee\
  \ doesnt use the token resource that is\n      in the oauth2 spec\", indicating the TOL API is (or was) fronted by Apigee with a non-standard\n      refresh endpoint.\ntoken_transport: Authorization bearer header on every request\ntoken_refresh: >-\n  Clients re-authenticate automatically on HTTP 401 with body error \"invalid_grant\"\n  (tol-api-nodejs isExpiredToken()).\nscopes:\n  documented: false\n  note: >-\n    No scope or permission reference is published. tol-api-nodejs exposes\n    handleGenericTokenWithScope(), so the TOL API supports scoped tokens, but the scope vocabulary is\n    not public. No scopes/ artifact is written rather than inventing scope names.\ncredential_issuance: >-\n  Not self-serve. Client id / client secret are issued to dealers and syndication partners through the\n  TraderTraxx dealer relationship; there is no public signup for API credentials.\ngaps:\n  - No published authentication documentation on any Trader Interactive property.\n  - No /.well-known/oauth-authorization-server\
  \ or /.well-known/openid-configuration on any host.\n  - Token endpoint path is documented only as \"{baseUrl}/token\" in client source; not independently verifiable anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trader-interactive/refs/heads/main/authentication/trader-interactive-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Marketplace
- Classifieds
- Automotive
- Power-Sports
- Recreational Vehicles
- Commercial Trucks
- Heavy Equipment
- Dealer Services
- Digital Advertising
- Vehicle Listings
- Media
---
