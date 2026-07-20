---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Better Mortgage Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Better Mortgage secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Better Mortgage
provider_slug: better-mortgage
scheme_count: 1
schemes:
- authorization_endpoint: https://prod.bettermg.com/api/idp/sso
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://prod.idp.bettermg.com/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw
  jwks_uri: https://prod.bettermg.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://www.better.com/.well-known/openid-configuration
  registration_endpoint: https://prod.bettermg.com/api/idp/sso/registration
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://prod.idp.bettermg.com/oauth2/revoke
  sources:
  - well-known/better-mortgage-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://prod.bettermg.com/api/idp/token
  token_endpoint_auth_methods_supported:
  - none
  type: openIdConnect
  userinfo_endpoint: https://prod.idp.bettermg.com/oauth2/userInfo
slug: better-mortgage-authentication
source_filename: better-mortgage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.better.com/.well-known/openid-configuration\ndocs: https://www.better.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, implicit]\n  identity_provider: AWS Cognito\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw\n  openIdConnectUrl: https://www.better.com/.well-known/openid-configuration\n  authorization_endpoint: https://prod.bettermg.com/api/idp/sso\n  token_endpoint: https://prod.bettermg.com/api/idp/token\n  userinfo_endpoint: https://prod.idp.bettermg.com/oauth2/userInfo\n  jwks_uri: https://prod.bettermg.com/.well-known/jwks.json\n  end_session_endpoint: https://prod.idp.bettermg.com/logout\n  registration_endpoint: https://prod.bettermg.com/api/idp/sso/registration\n  revocation_endpoint: https://prod.idp.bettermg.com/oauth2/revoke\n  response_types_supported:\
  \ [code, token]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  subject_types_supported: [public]\n  sources: [well-known/better-mortgage-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-mortgage/refs/heads/main/authentication/better-mortgage-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Fintech
- Mortgage
- Lending
- Real Estate
- Home Finance
- HELOC
- OpenID Connect
---
