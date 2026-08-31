---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sygnum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sygnum declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sygnum
provider_slug: sygnum
scheme_count: 2
schemes:
- audience: per-contract Auth0 audience, shown in the portal's Access Management screen
  client_authentication:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - none
  evidence:
    http_status: 401
    url: https://api.sygnum.com/b2b/v1/available-scopes
    www_authenticate: Bearer realm="auth.sygnum.com", error="invalid_token"
  flow: clientCredentials
  format: Bearer <access_token>
  header: Authorization
  id: oauth2_client_credentials
  in: header
  issuer: https://auth.sygnum.com/
  jwks_uri: https://auth.sygnum.com/.well-known/jwks.json
  note: The portal's credential form asks for a key identifier (kid), a PUBLIC KEY or CERTIFICATE and an expiry time, which is the private_key_jwt client-authentication method advertised in the discovery document.
  token_endpoint: https://auth.sygnum.com/oauth/token
  type: oauth2
- authorization_endpoint: https://auth.sygnum.com/authorize
  end_session_endpoint: https://auth.sygnum.com/oidc/logout
  id: oidc_user_login
  note: Human login to the developer portal itself. Authorization Code with PKCE (S256 and plain advertised); MFA challenge endpoint present.
  openIdConnectUrl: https://auth.sygnum.com/.well-known/openid-configuration
  revocation_endpoint: https://auth.sygnum.com/oauth/revoke
  type: openIdConnect
  userinfo_endpoint: https://auth.sygnum.com/userinfo
slug: sygnum-authentication
source_filename: sygnum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://auth.sygnum.com/.well-known/openid-configuration (HTTP 200) plus the\n  WWW-Authenticate challenge returned by https://api.sygnum.com/b2b/v1/available-scopes\n  (HTTP 401) and the Access Management copy published in the developer.sygnum.com bundle\nnote: >-\n  Sygnum publishes no OpenAPI, so this profile is not derived from a securitySchemes block.\n  Every field below was read from a live anonymous probe of the bank's own hosts.\nsummary: >-\n  OAuth 2.0 bearer tokens issued by Sygnum's Auth0 tenant at auth.sygnum.com. B2B partners\n  self-service their machine clients in the developer portal's Access Management screen:\n  each Auth0 client is created against a contract, given one or more credentials (a public\n  key or certificate with a key identifier and an expiry time) and scoped to the Sygnum\n  APIs it may call.\nschemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  in: header\n\
  \  header: Authorization\n  format: Bearer <access_token>\n  token_endpoint: https://auth.sygnum.com/oauth/token\n  issuer: https://auth.sygnum.com/\n  jwks_uri: https://auth.sygnum.com/.well-known/jwks.json\n  audience: per-contract Auth0 audience, shown in the portal's Access Management screen\n  client_authentication:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - none\n  note: >-\n    The portal's credential form asks for a key identifier (kid), a PUBLIC KEY or\n    CERTIFICATE and an expiry time, which is the private_key_jwt client-authentication\n    method advertised in the discovery document.\n  evidence:\n    url: https://api.sygnum.com/b2b/v1/available-scopes\n    http_status: 401\n    www_authenticate: 'Bearer realm=\"auth.sygnum.com\", error=\"invalid_token\"'\n- id: oidc_user_login\n  type: openIdConnect\n  openIdConnectUrl: https://auth.sygnum.com/.well-known/openid-configuration\n  note: >-\n    Human login to the developer portal itself. Authorization\
  \ Code with PKCE (S256 and\n    plain advertised); MFA challenge endpoint present.\n  authorization_endpoint: https://auth.sygnum.com/authorize\n  userinfo_endpoint: https://auth.sygnum.com/userinfo\n  end_session_endpoint: https://auth.sygnum.com/oidc/logout\n  revocation_endpoint: https://auth.sygnum.com/oauth/revoke\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- implicit\n- password\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\ntoken_signing_algs:\n- RS256\n- RS384\n- PS256\npkce_methods:\n- S256\n- plain\nmtls: false\napi_keys:\n  used: partial\n  note: >-\n    Portal copy (\"the API key will appear in the overview section of the specific requested\n    API in the developer portal\") indicates a per-API key is also surfaced to onboarded\n    clients alongside the OAuth client. The key's transport header is not published\n    publicly and was\
  \ not observed on any anonymous response.\ndocs: https://developer.sygnum.com/how-to-connect\ngated:\n  is_gated: true\n  detail: >-\n    The specification downloads and the Access Management screen require an authenticated\n    Sygnum client login; only the OIDC discovery document and the 401 challenge are\n    anonymous.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sygnum/refs/heads/main/authentication/sygnum-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Banking
- Digital Assets
- Cryptocurrency
- Custody
- Trading
- Staking
- Tokenization
- Settlement
- Market Data
- Financial Services
- Switzerland
- Singapore
- B2B
---
