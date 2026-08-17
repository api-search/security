---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Quad Graphics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- hybrid
overview: Quad/Graphics secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and hybrid flow(s).
provider_name: Quad/Graphics
provider_slug: quad-graphics
scheme_count: 1
schemes:
- applies_to: At-Home Connect (https://athomeconnect.quad.com/)
  authorization_endpoint: https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/authorize
  claims_supported:
  - name
  - given_name
  - family_name
  - email
  - sub
  - tid
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  end_session_endpoint: https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://quadb2c.b2clogin.com/d3a40049-07f8-47ef-93a3-3465ce8af90a/v2.0/
  jwks_uri: https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/discovery/v2.0/keys
  name: quad-b2c-cloverleaf-production
  openIdConnectUrl: https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/B2C_1A_Cloverleaf_Production_SignUpOrSignIn/v2.0/.well-known/openid-configuration
  policy: B2C_1A_Cloverleaf_Production_SignUpOrSignIn
  protocol: OpenID Connect 1.0 / OAuth 2.0
  provider: Microsoft Entra External ID (Azure AD B2C)
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  scopes_supported:
  - openid
  sources:
  - well-known/quad-graphics-b2c-openid-configuration.json
  subject_types_supported:
  - pairwise
  tenant: quadb2c.onmicrosoft.com
  token_endpoint: https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/token
  type: openIdConnect
slug: quad-graphics-authentication
source_filename: quad-graphics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/B2C_1A_Cloverleaf_Production_SignUpOrSignIn/v2.0/.well-known/openid-configuration\ndocs: https://www.quad.com/solutions/technology/at-home-connect\nnote: >-\n  Quad publishes no developer portal and no API reference, so there is no documented\n  auth model for its APIs. What IS anonymously verifiable is the identity layer in\n  front of the At-Home Connect self-service platform: the platform's SPA at\n  athomeconnect.quad.com bootstraps against Microsoft Entra External ID (Azure AD B2C)\n  in Quad's own `quadb2c.onmicrosoft.com` tenant, whose OIDC discovery document is\n  public and was fetched (HTTP 200). The scheme below is read verbatim from that\n  discovery document — it is the login for the product Quad markets as API-integrable,\n  not a published API authentication contract. The postal API host\n  (api.postal.quad.com) returns 403 to anonymous requests and publishes\
  \ no\n  WWW-Authenticate challenge, so its auth model could not be established.\nsummary:\n  types: [openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, hybrid]\n  developer_facing_auth_documented: false\nschemes:\n  - name: quad-b2c-cloverleaf-production\n    type: openIdConnect\n    protocol: OpenID Connect 1.0 / OAuth 2.0\n    provider: Microsoft Entra External ID (Azure AD B2C)\n    tenant: quadb2c.onmicrosoft.com\n    policy: B2C_1A_Cloverleaf_Production_SignUpOrSignIn\n    applies_to: At-Home Connect (https://athomeconnect.quad.com/)\n    issuer: https://quadb2c.b2clogin.com/d3a40049-07f8-47ef-93a3-3465ce8af90a/v2.0/\n    openIdConnectUrl: >-\n      https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/B2C_1A_Cloverleaf_Production_SignUpOrSignIn/v2.0/.well-known/openid-configuration\n    authorization_endpoint: >-\n      https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/authorize\n    token_endpoint:\
  \ >-\n      https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/token\n    end_session_endpoint: >-\n      https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/oauth2/v2.0/logout\n    jwks_uri: >-\n      https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/b2c_1a_cloverleaf_production_signuporsignin/discovery/v2.0/keys\n    response_types_supported:\n      - code\n      - code id_token\n      - code token\n      - code id_token token\n      - id_token\n      - id_token token\n      - token\n      - token id_token\n    scopes_supported: [openid]\n    subject_types_supported: [pairwise]\n    id_token_signing_alg_values_supported: [RS256]\n    claims_supported: [name, given_name, family_name, email, sub, tid, iss, iat, exp, aud, acr, nonce, auth_time]\n    sources: [well-known/quad-graphics-b2c-openid-configuration.json]\nunresolved:\n  - host: https://api.postal.quad.com\n    observed: HTTP\
  \ 403 at /, HTTP 404 on unknown paths, no WWW-Authenticate header\n    note: real Quad API host, but no anonymous auth discovery and no public reference\n  - host: https://connect.qg.com\n    observed: HTTP 401 on every path\n    note: Client Connect customer portal; credentials required before anything is readable\nx-evidence:\n  - {url: 'https://quadb2c.b2clogin.com/quadb2c.onmicrosoft.com/B2C_1A_Cloverleaf_Production_SignUpOrSignIn/v2.0/.well-known/openid-configuration', status: 200, fetched: '2026-08-13'}\n  - {url: 'https://athomeconnect.quad.com/', status: 200, fetched: '2026-08-13'}\n  - {url: 'https://api.postal.quad.com/', status: 403, fetched: '2026-08-13'}\n  - {url: 'https://connect.qg.com/openapi.json', status: 401, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quad-graphics/refs/heads/main/authentication/quad-graphics-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Marketing
- Print
- Media
- Advertising
- Direct Mail
- Marketing Technology
- Retail Media
- Packaging
- Data
---
