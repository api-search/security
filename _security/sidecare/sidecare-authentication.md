---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sidecare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SideCare secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SideCare
provider_slug: sidecare
scheme_count: 1
schemes:
- authorization_endpoint: https://www.sidecare.com/accounts/oauth/authorizations
  claims_supported:
  - iss
  - sub
  - aud
  - nonce
  - exp
  - iat
  - name
  - given_name
  - family_name
  - birthdate
  - phone_number
  - email
  - email_verified
  - address
  end_session_endpoint: https://www.sidecare.com/accounts/oauth/sessions/logout
  grant_types_supported:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.sidecare.com
  jwks_uri: https://www.sidecare.com/accounts/oauth/jwks.json
  name: sidecare-oidc
  openIdConnectUrl: https://www.sidecare.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - profile
  - email
  - address
  sources:
  - well-known/sidecare-openid-configuration.json
  token_endpoint: https://www.sidecare.com/accounts/oauth/tokens
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://www.sidecare.com/accounts/oauth/user_info
slug: sidecare-authentication
source_filename: sidecare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.sidecare.com/.well-known/openid-configuration\ndocs: https://www.sidecare.com/connexion-hub\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    SideCare operates an OpenID Connect provider (\"Sign in with SideCare\")\n    discovered via /.well-known/openid-configuration. No public developer\n    API with documented securitySchemes was found; this profiles the OIDC\n    identity surface only.\nschemes:\n- name: sidecare-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.sidecare.com/.well-known/openid-configuration\n  issuer: https://www.sidecare.com\n  authorization_endpoint: https://www.sidecare.com/accounts/oauth/authorizations\n  token_endpoint: https://www.sidecare.com/accounts/oauth/tokens\n  userinfo_endpoint: https://www.sidecare.com/accounts/oauth/user_info\n  jwks_uri: https://www.sidecare.com/accounts/oauth/jwks.json\n  end_session_endpoint: https://www.sidecare.com/accounts/oauth/sessions/logout\n\
  \  response_types_supported: [code]\n  grant_types_supported: [authorization_code]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  scopes_supported: [openid, profile, email, address]\n  claims_supported: [iss, sub, aud, nonce, exp, iat, name, given_name, family_name, birthdate, phone_number, email, email_verified, address]\n  sources: [well-known/sidecare-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidecare/refs/heads/main/authentication/sidecare-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Financial Services
- Insurance
- Insurtech
- Health Insurance
- Employee Benefits
- Human Resources
- HRIS
- France
- OpenID Connect
---
