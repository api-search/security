---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: artsy-public-api-openapi.yml
  format: yaml
  label: Artsy Public API
  slug: artsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artsy/refs/heads/main/openapi/artsy-public-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Artsy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
- custom-oauth_token-exchange
overview: Artsy secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, password, and custom-oauth_token-exchange flow(s).
provider_name: Artsy
provider_slug: artsy
scheme_count: 3
schemes:
- description: Anonymous application-level token. Obtained by POSTing client_id and client_secret to /api/tokens/xapp_token; the response carries type, token and expires_at. This is the token most public-domain read traffic uses — no user account required.
  in: header
  name: XappToken
  parameter_name: X-Xapp-Token
  source_operation: openapi/artsy-public-api-openapi.yml#postApiTokensXappToken
  sources:
  - https://developers.artsy.net/v2/docs/authentication
  token_endpoint: https://api.artsy.net/api/tokens/xapp_token
  type: apiKey
- description: User-scoped token returned by every /oauth2/access_token grant below. Revoked by DELETE /api/tokens/access_token.
  in: header
  name: UserAccessToken
  parameter_name: X-Auth-Token
  revocation_operation: openapi/artsy-public-api-openapi.yml#deleteApiTokensAccessToken
  sources:
  - https://developers.artsy.net/v2/docs/authentication
  type: apiKey
- description: Artsy acts as an OAuth 2 provider for user login. Redirect URIs are NOT restricted per application and the provider states users are prompted to trust the application on every login — documented as a known limitation, not a configuration option.
  flows:
  - authorizationUrl: https://api.artsy.net/oauth2/authorize
    flow: authorizationCode
    grant_type: authorization_code
    parameters:
    - client_id
    - client_secret
    - code
    - grant_type
    - state
    - scope
    tokenUrl: https://api.artsy.net/oauth2/access_token
  - flow: password
    grant_type: credentials
    note: Email/password exchange. The provider's own documentation says this is "not recommended".
    parameters:
    - client_id
    - client_secret
    - grant_type
    - email
    - password
    - scope
    tokenUrl: https://api.artsy.net/oauth2/access_token
  - flow: token-exchange
    grant_type: oauth_token
    note: Non-standard grant that exchanges a Facebook or Twitter social token for an Artsy token. oauth_provider is either "facebook" or "twitter".
    parameters:
    - client_id
    - client_secret
    - grant_type
    - oauth_token
    - oauth_token_secret
    - oauth_provider
    tokenUrl: https://api.artsy.net/oauth2/access_token
  name: OAuth2
  sources:
  - https://developers.artsy.net/v2/docs/authentication
  type: oauth2
slug: artsy-authentication
source_filename: artsy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://developers.artsy.net/v2/docs/authentication\ndocs: https://developers.artsy.net/v2/docs/authentication\nnote: >-\n  The harvested Swagger 2.0 contract at https://api.artsy.net/api/docs/ declares NO securityDefinitions,\n  so derive-authentication.py found nothing to aggregate. This profile is read from the provider's own\n  authentication documentation instead, which describes four token mechanisms in prose. Nothing here is\n  inferred: every scheme, endpoint, header name and lifetime below is stated on that page.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, password, custom-oauth_token-exchange]\n  spec_declares_security: false\ncredentials:\n  registration: https://developers.artsy.net/v2/docs/getting-started\n  console: https://developers.artsy.net/client_applications\n  issued: client_id + client_secret, per client application\nschemes:\n  - name: XappToken\n\
  \    type: apiKey\n    in: header\n    parameter_name: X-Xapp-Token\n    description: >-\n      Anonymous application-level token. Obtained by POSTing client_id and client_secret to\n      /api/tokens/xapp_token; the response carries type, token and expires_at. This is the token most\n      public-domain read traffic uses — no user account required.\n    token_endpoint: https://api.artsy.net/api/tokens/xapp_token\n    source_operation: openapi/artsy-public-api-openapi.yml#postApiTokensXappToken\n    sources: [https://developers.artsy.net/v2/docs/authentication]\n  - name: UserAccessToken\n    type: apiKey\n    in: header\n    parameter_name: X-Auth-Token\n    description: >-\n      User-scoped token returned by every /oauth2/access_token grant below. Revoked by\n      DELETE /api/tokens/access_token.\n    revocation_operation: openapi/artsy-public-api-openapi.yml#deleteApiTokensAccessToken\n    sources: [https://developers.artsy.net/v2/docs/authentication]\n  - name: OAuth2\n    type:\
  \ oauth2\n    description: >-\n      Artsy acts as an OAuth 2 provider for user login. Redirect URIs are NOT restricted per\n      application and the provider states users are prompted to trust the application on every login\n      — documented as a known limitation, not a configuration option.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.artsy.net/oauth2/authorize\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n        grant_type: authorization_code\n        parameters: [client_id, client_secret, code, grant_type, state, scope]\n      - flow: password\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n        grant_type: credentials\n        parameters: [client_id, client_secret, grant_type, email, password, scope]\n        note: >-\n          Email/password exchange. The provider's own documentation says this is \"not recommended\".\n      - flow: token-exchange\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n\
  \        grant_type: oauth_token\n        parameters: [client_id, client_secret, grant_type, oauth_token, oauth_token_secret, oauth_provider]\n        note: >-\n          Non-standard grant that exchanges a Facebook or Twitter social token for an Artsy token.\n          oauth_provider is either \"facebook\" or \"twitter\".\n    sources: [https://developers.artsy.net/v2/docs/authentication]\ntoken_lifetime:\n  default: 60 days\n  offline_access: 25 years\n  note: >-\n    Verbatim from the provider: setting scope to \"offline_access\" requests a token that expires in\n    25 years instead of the standard 60 days. XAPP tokens carry their own expires_at in the response.\nerror_envelope:\n  fields: [error, error_description]\n  note: OAuth 2 error code plus a human-readable description, per the authentication page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artsy/refs/heads/main/authentication/artsy-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Art
- Marketplace
- Artists
- Collectors
- Galleries
- Auctions
- Museums
- Art Market
- Culture
- Images
---
