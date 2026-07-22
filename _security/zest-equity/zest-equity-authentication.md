---
api_key_in: []
api_specs:
- filename: zest-equity-openapi-original.json
  format: json
  label: Zest Public API
  slug: zest-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zest-equity/refs/heads/main/openapi/zest-equity-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zest Equity Authentication
name_suffix: Authentication
oauth_flows:
- jwt-bearer-assertion
- refresh_token
overview: Zest Equity secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the jwt-bearer-assertion and refresh_token flow(s).
provider_name: Zest Equity
provider_slug: zest-equity
scheme_count: 2
schemes:
- description: Every partner API call presents a short-lived bearer access token in the Authorization header. Tokens are minted via the OAuth 2.0 JWT-Bearer assertion grant (RFC 7523), not issued directly.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/zest-equity-openapi-original.json
  type: http
- assertion_claims:
    aud: Exactly the Zest environment base URL — https://public-api.zestequity.com or https://sandbox-api.zestequity.com
    client_id: Your client_id (must equal sub)
    exp: Expiry (unix seconds; ~60s recommended)
    iat: Issued-at (unix seconds)
    iss: Your API base URL (issuer identifier)
    sub: Your client_id (must equal client_id claim)
  description: Partners sign a JWT assertion with their registered EdDSA (Ed25519) private key and POST it to /v1/oauth2/tokens with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer to receive an access token + refresh token. Only EdDSA is accepted; RSA/HMAC assertions are rejected.
  introspection: GET /v1/oauth2/info (returns client type, client id, application name)
  name: OAuth2 JWT-Bearer assertion
  sandbox_token_url: https://sandbox-api.zestequity.com/v1/oauth2/tokens
  sources:
  - https://docs.zestequity.com/authentication
  standard: RFC 7523
  token_response:
    access_token_ttl_seconds: 3600
    notes: Refresh tokens rotate on every use; redeeming a stale refresh token returns 401 and invalidates the whole chain, forcing a fresh JWT-bearer assertion.
    refresh_rotates: true
    refresh_token_ttl_seconds: 2592000
    token_type: Bearer
  token_url: https://public-api.zestequity.com/v1/oauth2/tokens
  type: oauth2
slug: zest-equity-authentication
source_filename: zest-equity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zest-equity-openapi-original.json\ndocs: https://docs.zestequity.com/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - jwt-bearer-assertion\n  - refresh_token\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: >-\n    Every partner API call presents a short-lived bearer access token in the\n    Authorization header. Tokens are minted via the OAuth 2.0 JWT-Bearer\n    assertion grant (RFC 7523), not issued directly.\n  sources:\n  - openapi/zest-equity-openapi-original.json\n- name: OAuth2 JWT-Bearer assertion\n  type: oauth2\n  standard: RFC 7523\n  description: >-\n    Partners sign a JWT assertion with their registered EdDSA (Ed25519) private\n    key and POST it to /v1/oauth2/tokens with\n    grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer to receive an access\n    token + refresh token. Only EdDSA is accepted; RSA/HMAC assertions are\n\
  \    rejected.\n  token_url: https://public-api.zestequity.com/v1/oauth2/tokens\n  sandbox_token_url: https://sandbox-api.zestequity.com/v1/oauth2/tokens\n  assertion_claims:\n    iss: Your API base URL (issuer identifier)\n    sub: Your client_id (must equal client_id claim)\n    aud: >-\n      Exactly the Zest environment base URL —\n      https://public-api.zestequity.com or https://sandbox-api.zestequity.com\n    client_id: Your client_id (must equal sub)\n    iat: Issued-at (unix seconds)\n    exp: Expiry (unix seconds; ~60s recommended)\n  token_response:\n    access_token_ttl_seconds: 3600\n    refresh_token_ttl_seconds: 2592000\n    token_type: Bearer\n    refresh_rotates: true\n    notes: >-\n      Refresh tokens rotate on every use; redeeming a stale refresh token\n      returns 401 and invalidates the whole chain, forcing a fresh JWT-bearer\n      assertion.\n  introspection: GET /v1/oauth2/info (returns client type, client id, application name)\n  sources:\n  - https://docs.zestequity.com/authentication\n\
  notes: >-\n  The OpenAPI declares only the HTTPBearer http/bearer scheme; the JWT-Bearer\n  assertion token-minting flow is documented (RFC 7523) but not modelled as an\n  oauth2 securityScheme in the spec. Provisioning (client_id + EdDSA key) is\n  done during partner onboarding via sara@zestholdco.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zest-equity/refs/heads/main/authentication/zest-equity-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Private Markets
- SPV
- Investments
- Escrow
- Fund Administration
- MENA
- Webhooks
- Regulated
---
