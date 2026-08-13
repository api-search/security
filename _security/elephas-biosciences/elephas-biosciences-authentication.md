---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: probed
name: Elephas Biosciences Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Elephas Biosciences secures its APIs with oauth2, openIdConnect, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Elephas Biosciences
provider_slug: elephas-biosciences
scheme_count: 2
schemes:
- applies_to: every path on https://portal.elephasapis.com, including /swagger and /.well-known/*
  bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  source: 'observed: WWW-Authenticate: Bearer on HTTP 401 from https://portal.elephasapis.com/swagger'
  type: http
- authorization_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/authorize
  claims_supported:
  - firstname
  - surname
  - idp
  - email
  - sub
  - identityProviders
  - isForgotPassword
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  end_session_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/logout
  federation: The SMART_HRD policy name plus the identityProviders and idp claims indicate home-realm discovery — institutional users are federated to their own identity provider rather than holding local Elephas credentials.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/v2.0/
  jwks_uri: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/discovery/v2.0/keys
  name: AzureAdB2C
  openIdConnectUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/B2C_1A_SMART_HRD_SUSI/v2.0/.well-known/openid-configuration
  policy: B2C_1A_SMART_HRD_SUSI
  policy_kind: custom policy (Identity Experience Framework), home-realm-discovery sign-up/sign-in
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  source: well-known/elephas-biosciences-openid-configuration.json
  subject_types_supported:
  - pairwise
  token_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
slug: elephas-biosciences-authentication
source_filename: elephas-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: 'https://portal.elephas.com/assets/config/config.json (portal runtime\n  config) + https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/B2C_1A_SMART_HRD_SUSI/v2.0/.well-known/openid-configuration\n  + observed WWW-Authenticate challenge on https://portal.elephasapis.com'\nnote: 'DERIVED FROM PROBES, NOT FROM A PUBLISHED SPEC OR AUTH DOC. Elephas publishes\n  no developer documentation and no OpenAPI, so there are no securitySchemes to\n  read. Everything below was observed live: the Bearer challenge on the API host,\n  and the OpenID Connect discovery metadata the company''s own Azure AD B2C identity\n  host serves anonymously.'\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  identity_provider: Azure AD B2C (custom domain)\n  public_registration: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  source: 'observed:\
  \ WWW-Authenticate: Bearer on HTTP 401 from\n    https://portal.elephasapis.com/swagger'\n  applies_to: every path on https://portal.elephasapis.com, including /swagger and\n    /.well-known/*\n- name: AzureAdB2C\n  type: openIdConnect\n  openIdConnectUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/B2C_1A_SMART_HRD_SUSI/v2.0/.well-known/openid-configuration\n  issuer: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/v2.0/\n  authorization_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/authorize\n  token_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token\n  end_session_endpoint: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/logout\n  jwks_uri: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/discovery/v2.0/keys\n  policy: B2C_1A_SMART_HRD_SUSI\n\
  \  policy_kind: custom policy (Identity Experience Framework), home-realm-discovery\n    sign-up/sign-in\n  response_types_supported: [code, code id_token, code token, code id_token token,\n    id_token, id_token token, token, token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  claims_supported: [firstname, surname, idp, email, sub, identityProviders,\n    isForgotPassword, iss, iat, exp, aud, acr, nonce, auth_time]\n  federation: 'The SMART_HRD policy name plus the identityProviders and idp claims\n    indicate home-realm discovery — institutional users are federated to their own\n    identity provider rather than holding local Elephas credentials.'\n  source: well-known/elephas-biosciences-openid-configuration.json\nclient:\n  type: public (browser SPA, MSAL.js)\n  flow: authorization code\
  \ with PKCE\n  note: The Elephas Portal is an Angular application using MSAL; the client id is\n    public by construction and is intentionally not recorded here.\ngaps:\n- No published authentication documentation, developer portal, or token-issuance\n  guide exists on any Elephas host.\n- The discovery document advertises implicit and hybrid response types (token,\n  id_token token) alongside authorization code; this is Azure AD B2C's default\n  advertisement, not necessarily an enabled application configuration.\n- scopes_supported in the discovery document lists only \"openid\"; the resource scope\n  is configured on the application rather than advertised. See\n  scopes/elephas-biosciences-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elephas-biosciences/refs/heads/main/authentication/elephas-biosciences-authentication.yml
summary_line: oauth2/openIdConnect/http · 2 schemes
tags:
- Company
- Healthcare
- Life Sciences
- Biotechnology
- Precision Oncology
- Diagnostics
- Immunotherapy
- Clinical Research
- Laboratory
- Medical Devices
---
