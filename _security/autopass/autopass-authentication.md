---
api_key_in: []
api_specs:
- filename: autopass-openapi.yml
  format: yaml
  label: Autopass Service Authorization API
  slug: autopass-service-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/openapi/autopass-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Autopass Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- refresh_token
overview: Autopass secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and refresh_token flow(s).
provider_name: Autopass
provider_slug: autopass
scheme_count: 2
schemes:
- authorization_endpoint: https://api.autopass.xyz/oauth/authorize
  grant_types:
  - client_credentials
  - password
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://api.autopass.xyz/oauth/introspect
  jwks_uri: https://api.autopass.xyz/oauth/discovery/keys
  name: autopassOAuth
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  revocation_endpoint: https://api.autopass.xyz/oauth/revoke
  source: https://api.autopass.xyz/.well-known/openid-configuration
  subject_types:
  - public
  token_endpoint: https://api.autopass.xyz/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://api.autopass.xyz/oauth/userinfo
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - email
  - email_verified
  - phone_number
  - phone_number_verified
  name: autopassOIDC
  openIdConnectUrl: https://api.autopass.xyz/.well-known/openid-configuration
  type: openIdConnect
slug: autopass-authentication
source_filename: autopass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.autopass.xyz/.well-known/openid-configuration\ndocs: https://docs.autopass.xyz/autopass-fu-wu-shou-quan-fang-an.md\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, password, refresh_token]\n  api_key_in: []\nissuer: https://www.autopass.xyz\nschemes:\n  - name: autopassOAuth\n    type: oauth2\n    source: https://api.autopass.xyz/.well-known/openid-configuration\n    authorization_endpoint: https://api.autopass.xyz/oauth/authorize\n    token_endpoint: https://api.autopass.xyz/oauth/token\n    revocation_endpoint: https://api.autopass.xyz/oauth/revoke\n    introspection_endpoint: https://api.autopass.xyz/oauth/introspect\n    userinfo_endpoint: https://api.autopass.xyz/oauth/userinfo\n    jwks_uri: https://api.autopass.xyz/oauth/discovery/keys\n    grant_types: [client_credentials, password, authorization_code, refresh_token]\n    response_types: [code]\n    response_modes:\
  \ [query, fragment, form_post]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n  - name: autopassOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://api.autopass.xyz/.well-known/openid-configuration\n    claims_supported: [iss, sub, aud, exp, iat, email, email_verified, phone_number, phone_number_verified]\nnotes: >-\n  OAuth 2.0 Authorization Code + Client Credentials are the primary partner flows; password\n  and refresh_token grants are also advertised. OpenID Connect discovery exposes a single\n  'openid' scope. Bearer access tokens are presented to the resource API at api.autopass.xyz.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/authentication/autopass-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Mobility
- Parking
- Payments
- Automotive
- Financial Services
- OAuth
- Taiwan
---
