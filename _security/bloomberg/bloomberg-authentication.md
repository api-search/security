---
api_key_in: []
api_specs:
- filename: bloomberg-reference-data-api-openapi.yml
  format: yaml
  label: Bloomberg BLPAPI Core
  slug: bloomberg-blpapi-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/openapi/bloomberg-reference-data-api-openapi.yml
auth_types:
- session-identity
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bloomberg Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Bloomberg secures its APIs with session-identity, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Bloomberg
provider_slug: bloomberg
scheme_count: 3
schemes:
- description: Desktop API — the BLPAPI SDK connects to localhost:8194 and inherits the identity of the logged-in Bloomberg Professional (Terminal) user. No separate credentials are exchanged.
  name: DesktopAPISession
  sources:
  - openapi/bloomberg-reference-data-api-openapi.yml
  type: session-identity
- description: Server API (SAPI) / B-PIPE — applications authorize users and applications through the //blp/apiauth service (AuthorizationRequest), producing Identity objects attached to requests and subscriptions. The SDK models this as AuthOptions / AuthUser / Identity (see the Python SDK reference). Entitlements (EIDs) gate which data an identity may receive.
  docs: https://bloomberg.github.io/blpapi-docs/python/3.26.6/
  name: ServerApiAuthorization
  type: session-identity
- description: OAuth 2.0 / OIDC for Bloomberg web login and HTTP-delivered services — RFC 8414 metadata published at www.bloomberg.com/.well-known/oauth-authorization-server; authorization and token endpoints on login.bloomberg.com; authorization_code + refresh_token grants with PKCE (S256); scopes openid, user, entitlements. See scopes/bloomberg-scopes.yml.
  flows:
  - authorizationUrl: https://login.bloomberg.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.bloomberg.com/api/oauth/token
  name: BloombergOAuth
  sources:
  - well-known/bloomberg-oauth-authorization-server.json
  type: oauth2
slug: bloomberg-authentication
source_filename: bloomberg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://bloomberg.github.io/blpapi-docs/ (BLPAPI Core Developer/User Guides, SDK AuthOptions/AuthUser/Identity) + https://www.bloomberg.com/.well-known/oauth-authorization-server\ndocs: https://bloomberg.github.io/blpapi-docs/\nnotes: >-\n  The BLPAPI OpenAPI projections in this repo declare no HTTP securitySchemes because BLPAPI is a\n  socket/SDK API — authentication is session- and identity-based, not header-based. The derive pass\n  (derive-authentication.py) therefore found 0 schemes; this profile is searched from the SDK docs\n  and Bloomberg's published OAuth discovery metadata.\nsummary:\n  types: [session-identity, oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken]\nschemes:\n  - name: DesktopAPISession\n    type: session-identity\n    description: >-\n      Desktop API — the BLPAPI SDK connects to localhost:8194 and inherits the identity of the\n      logged-in Bloomberg Professional (Terminal)\
  \ user. No separate credentials are exchanged.\n    sources: [openapi/bloomberg-reference-data-api-openapi.yml]\n  - name: ServerApiAuthorization\n    type: session-identity\n    description: >-\n      Server API (SAPI) / B-PIPE — applications authorize users and applications through the\n      //blp/apiauth service (AuthorizationRequest), producing Identity objects attached to requests\n      and subscriptions. The SDK models this as AuthOptions / AuthUser / Identity (see the Python SDK\n      reference). Entitlements (EIDs) gate which data an identity may receive.\n    docs: https://bloomberg.github.io/blpapi-docs/python/3.26.6/\n  - name: BloombergOAuth\n    type: oauth2\n    description: >-\n      OAuth 2.0 / OIDC for Bloomberg web login and HTTP-delivered services — RFC 8414 metadata\n      published at www.bloomberg.com/.well-known/oauth-authorization-server; authorization and token\n      endpoints on login.bloomberg.com; authorization_code + refresh_token grants with PKCE (S256);\n\
  \      scopes openid, user, entitlements. See scopes/bloomberg-scopes.yml.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.bloomberg.com/api/oauth/authorize\n        tokenUrl: https://login.bloomberg.com/api/oauth/token\n    sources: [well-known/bloomberg-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/authentication/bloomberg-authentication.yml
summary_line: session-identity/oauth2/openIdConnect · 3 schemes
tags:
- Analytics
- Business Intelligence
- Data License
- Enterprise
- Execution Management
- Financial Services
- Market Data
- News
- Quantitative Analysis
- Trading
- Transaction Cost Analysis
---
