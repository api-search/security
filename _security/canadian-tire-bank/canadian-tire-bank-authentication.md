---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Canadian Tire Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
overview: Canadian Tire Bank secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and refreshToken flow(s).
provider_name: Canadian Tire Bank
provider_slug: canadian-tire-bank
scheme_count: 2
schemes:
- authorization_endpoint: https://api.ctfs.com:443/auth/oauth/v2/authorize
  id_token_signing_alg_values_supported:
  - RS256
  - HS256
  issuer: https://api.ctfs.com
  jwks_uri: https://api.ctfs.com:443/openid/connect/jwks.json
  name: openIdConnect
  openIdConnectUrl: https://www.ctfs.com/.well-known/openid-configuration
  registration_endpoint: https://api.ctfs.com:443/openid/connect/register
  sources:
  - well-known/canadian-tire-bank-openid-configuration.json
  subject_types_supported:
  - pairwise
  token_endpoint: https://api.ctfs.com:443/auth/oauth/v2/token
  type: openIdConnect
  userinfo_endpoint: https://api.ctfs.com:443/openid/connect/v1/userinfo
- flows:
  - authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://api.ctfs.com:443/auth/oauth/v2/token
  - authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize
    flow: implicit
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  name: OAuth2
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - token id_token
  - token
  - code id_token
  - id_token
  - code token
  - code id_token token
  sources:
  - well-known/canadian-tire-bank-openid-configuration.json
  type: oauth2
slug: canadian-tire-bank-authentication
source_filename: canadian-tire-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.ctfs.com/.well-known/openid-configuration\ndocs: https://api.ctfs.com/apidocs/auth/oauth/v2/swagger  # HTTP 503 at probe time (2026-07-23)\nnotes: >-\n  Derived from the bank's anonymously-published OpenID Connect discovery\n  document. This is a CONSUMER-facing OAuth2/OIDC authorization server (Triangle\n  cardmember / account sign-in), not a documented public developer/banking API.\n  The scopes advertised (openid, email, profile) confirm a login/identity surface\n  rather than a data-access API. The issuer host api.ctfs.com returned HTTP 503 on\n  every probe, so token/authorize endpoints could not be exercised.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit, refreshToken]\n  oidc_issuer: https://api.ctfs.com\n  dynamic_client_registration: true    # registration_endpoint present (RFC 7591)\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt,\
  \ private_key_jwt]\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.ctfs.com/.well-known/openid-configuration\n  issuer: https://api.ctfs.com\n  authorization_endpoint: https://api.ctfs.com:443/auth/oauth/v2/authorize\n  token_endpoint: https://api.ctfs.com:443/auth/oauth/v2/token\n  userinfo_endpoint: https://api.ctfs.com:443/openid/connect/v1/userinfo\n  jwks_uri: https://api.ctfs.com:443/openid/connect/jwks.json\n  registration_endpoint: https://api.ctfs.com:443/openid/connect/register\n  id_token_signing_alg_values_supported: [RS256, HS256]\n  subject_types_supported: [pairwise]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize\n    tokenUrl: https://api.ctfs.com:443/auth/oauth/v2/token\n  - flow: implicit\n    authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize\n  grant_types_supported:\
  \ [authorization_code, implicit, refresh_token]\n  response_types_supported: [code, \"token id_token\", token, \"code id_token\", id_token, \"code token\", \"code id_token token\"]\n  response_modes_supported: [query, fragment, form_post]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-tire-bank/refs/heads/main/authentication/canadian-tire-bank-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Credit Cards
- Mastercard
- Consumer-Driven Banking
- Data Aggregation
---
