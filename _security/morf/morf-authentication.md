---
api_key_in:
- header
- query
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Morf Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Morf secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Morf
provider_slug: morf
scheme_count: 4
schemes:
- description: Primary server-to-server credential. Issued from the Morf Editor (request access keys — you are granted one site key and one API key). Sent in the API-Key request header. Keys are environment-scoped (sandbox vs live Morf environment).
  in: header
  name: ApiKey
  parameter_name: API-Key
  type: apiKey
- description: Publicly embeddable key passed as the siteKey query-string parameter. Meant for client-side/public contexts only; the docs warn it must NOT be used to access protected API services because it is designed to be public, unlike the API key.
  in: query
  name: SiteKey
  parameter_name: siteKey
  type: apiKey
- flows:
  - authorizationUrl: https://dashboard.morf.health/authorize
    flow: authorizationCode
    registrationUrl: https://auth.morf.health/v1/oauth2/register
    scopes_count: 6
    tokenUrl: https://auth.morf.health/v1/oauth2/token
  name: OAuth2
  sources:
  - well-known/morf-oauth-authorization-server.json
  type: oauth2
- id_token_signing_alg: RS256
  issuer: https://auth.morf.health
  jwks_uri: https://auth.morf.health/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://auth.morf.health/.well-known/openid-configuration
  pkce:
  - S256
  sources:
  - well-known/morf-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://auth.morf.health/v1/oauth2/userinfo
slug: morf-authentication
source_filename: morf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.morf.health/ + https://auth.morf.health/.well-known/openid-configuration\ndocs: https://docs.morf.health/\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter_name: API-Key\n  description: >-\n    Primary server-to-server credential. Issued from the Morf Editor (request\n    access keys — you are granted one site key and one API key). Sent in the\n    API-Key request header. Keys are environment-scoped (sandbox vs live Morf\n    environment).\n- name: SiteKey\n  type: apiKey\n  in: query\n  parameter_name: siteKey\n  description: >-\n    Publicly embeddable key passed as the siteKey query-string parameter. Meant\n    for client-side/public contexts only; the docs warn it must NOT be used to\n    access protected API services because it is designed to be public, unlike\n    the\
  \ API key.\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.morf.health/authorize\n    tokenUrl: https://auth.morf.health/v1/oauth2/token\n    registrationUrl: https://auth.morf.health/v1/oauth2/register\n    scopes_count: 6\n  sources: [well-known/morf-oauth-authorization-server.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.morf.health/.well-known/openid-configuration\n  issuer: https://auth.morf.health\n  userinfo_endpoint: https://auth.morf.health/v1/oauth2/userinfo\n  jwks_uri: https://auth.morf.health/.well-known/jwks.json\n  id_token_signing_alg: RS256\n  pkce: [S256]\n  sources: [well-known/morf-openid-configuration.json]\nnotes: >-\n  Auth model derived from published Morf docs and live OAuth/OIDC discovery\n  documents (no OpenAPI securitySchemes were retrievable — the API host returns\n  415 to unauthenticated spec requests). token_endpoint_auth_methods:\n  client_secret_basic,\
  \ client_secret_post, none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morf/refs/heads/main/authentication/morf-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Healthcare
- Health IT
- Automation
- Integration
- iPaaS
- Webhooks
- EHR
- Patient Communication
- HIPAA
- Workflow
- Digital Health
---
