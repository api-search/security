---
api_key_in: []
api_specs:
- filename: postman.yaml
  format: yaml
  label: Klutch Public API
  slug: klutch-public-api
  spec_type: Postman
  url: https://api-docs.klutchcard.com/
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Klutch Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Klutch secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Klutch
provider_slug: klutch
scheme_count: 4
schemes:
- description: 'Every Klutch GraphQL call carries `Authorization: Bearer <token>`. The collection-level auth in the published Postman collection is bearer.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - postman/klutch-public-api-postman.json
  type: http
- description: Developers exchange a client id and secret key for a session bearer token with the `createSessionToken` mutation, then send that token as the bearer on subsequent calls. Credentials are issued from the Klutch developer area ("My Account" -> "Developers") and are supplied to the samples as KLUTCH_CLIENT_ID / KLUTCH_SECRET_KEY environment variables.
  name: sessionToken
  operation: 'mutation($clientId: String, $secretKey: String) { createSessionToken(clientId: $clientId, secretKey: $secretKey) }'
  sources:
  - postman/klutch-public-api-postman.json
  - https://github.com/KlutchCard/api-samples
  type: credentials-exchange
- description: Klutch runs an OAuth 2.1 authorization server in front of each API host, advertised via RFC 8414 metadata. Authorization code with PKCE only (S256), public clients (token_endpoint_auth_methods_supported is "none"), with RFC 7591 dynamic client registration. This is the flow user-consented agents (including the Klutch MCP server) use. The underlying identity provider is Amazon Cognito.
  flows:
  - authorizationUrl: https://graphql.klutchcard.com/oauth/authorize
    endSessionUrl: https://auth.klutch.cards/logout
    flow: authorizationCode
    registrationUrl: https://graphql.klutchcard.com/oauth/register
    revocationUrl: https://auth.klutch.cards/oauth2/revoke
    scopes:
    - openid
    - email
    - phone
    - profile
    tokenUrl: https://graphql.klutchcard.com/oauth/token
    userinfoUrl: https://auth.klutch.cards/oauth2/userInfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_LSWgwjdrS
  jwks_uri: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_LSWgwjdrS/.well-known/jwks.json
  name: oauth2
  sources:
  - well-known/klutch-graphql-oauth-authorization-server.json
  type: oauth2
- description: Mini Apps are registered with a developer-generated key pair (`klutch generateKey` in the CLI) and sign a JWT to obtain a miniapp access token; that token mints a per-install token via `recipeInstall(id:) { createToken }`, which is the bearer used for panel mutations on behalf of an installing user.
  name: miniappJwt
  sources:
  - postman/klutch-public-api-postman.json
  - cli/klutch-cli.yml
  tokens:
  - miniapp_access_token
  - recipeinstall_token
  type: jwt-assertion
slug: klutch-authentication
source_filename: klutch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api-docs.klutchcard.com/ (Klutch Public API Postman collection),\n  well-known/klutch-graphql-oauth-authorization-server.json,\n  https://github.com/KlutchCard/api-samples\ndocs: https://www.klutchcard.com/developer\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  bearer_sources: [session-token-mutation, oauth2-authorization-code]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  dynamic_client_registration: true\n  pkce: S256\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Every Klutch GraphQL call carries `Authorization: Bearer <token>`. The\n    collection-level auth in the published Postman collection is bearer.\n  sources: [postman/klutch-public-api-postman.json]\n- name: sessionToken\n  type: credentials-exchange\n  description: >-\n    Developers exchange a client id and secret key for a session bearer token\
  \ with\n    the `createSessionToken` mutation, then send that token as the bearer on\n    subsequent calls. Credentials are issued from the Klutch developer area\n    (\"My Account\" -> \"Developers\") and are supplied to the samples as\n    KLUTCH_CLIENT_ID / KLUTCH_SECRET_KEY environment variables.\n  operation: 'mutation($clientId: String, $secretKey: String) { createSessionToken(clientId:\n    $clientId, secretKey: $secretKey) }'\n  sources: [postman/klutch-public-api-postman.json, 'https://github.com/KlutchCard/api-samples']\n- name: oauth2\n  type: oauth2\n  description: >-\n    Klutch runs an OAuth 2.1 authorization server in front of each API host, advertised\n    via RFC 8414 metadata. Authorization code with PKCE only (S256), public clients\n    (token_endpoint_auth_methods_supported is \"none\"), with RFC 7591 dynamic client\n    registration. This is the flow user-consented agents (including the Klutch MCP\n    server) use. The underlying identity provider is Amazon Cognito.\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://graphql.klutchcard.com/oauth/authorize\n    tokenUrl: https://graphql.klutchcard.com/oauth/token\n    registrationUrl: https://graphql.klutchcard.com/oauth/register\n    revocationUrl: https://auth.klutch.cards/oauth2/revoke\n    userinfoUrl: https://auth.klutch.cards/oauth2/userInfo\n    endSessionUrl: https://auth.klutch.cards/logout\n    scopes: [openid, email, phone, profile]\n  issuer: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_LSWgwjdrS\n  jwks_uri: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_LSWgwjdrS/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/klutch-graphql-oauth-authorization-server.json]\n- name: miniappJwt\n  type: jwt-assertion\n  description: >-\n    Mini Apps are registered with a developer-generated key pair (`klutch generateKey`\n    in the CLI) and sign a JWT to obtain a miniapp access token; that token mints a\n    per-install\
  \ token via `recipeInstall(id:) { createToken }`, which is the bearer\n    used for panel mutations on behalf of an installing user.\n  tokens:\n  - miniapp_access_token\n  - recipeinstall_token\n  sources: [postman/klutch-public-api-postman.json, cli/klutch-cli.yml]\nenvironments:\n- name: production\n  endpoint: https://graphql.klutchcard.com/graphql\n  audience: a user acting on their own data\n- name: sandbox\n  endpoint: https://sandbox.klutchcard.com/graphql\n  audience: Mini App developers testing from a multi-user perspective\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klutch/refs/heads/main/authentication/klutch-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Payments
- Card Issuing
- Virtual Cards
- Transactions
- Spend Management
- Personal Finance
- GraphQL
- Embedded Finance
- Agents
---
