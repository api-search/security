---
api_key_in:
- body
auth_types:
- oauth2
- custom-token
description: ''
kind: authentication
layout: security
method: searched
name: Fxiaoke Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Fxiaoke secures its APIs with oauth2 and custom-token across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Fxiaoke
provider_slug: fxiaoke
scheme_count: 2
schemes:
- caching_guidance: Token is valid for 2 hours (7200s). Callers must cache it for at least 6600s and refresh by re-calling the token endpoint between 6650s and 7200s; the token expires at 7200s.
  description: Self-built enterprise application flow. A tenant creates a self-built app in the Fxiaoke admin console (developer mode) and receives appId, appSecret, and a permanentCode. These are exchanged for a short-lived access token (called corpAccessToken / app access token) that authenticates all subsequent Open API v2 calls.
  flow: clientCredentials
  name: enterprise-app-token
  request:
    content_type: application/json
    fields:
    - name: appId
      required: true
    - name: appSecret
      required: true
    - name: permanentCode
      required: true
    - name: grantType
      required: true
      value: app_secret
    method: POST
  response_fields:
  - accessToken
  - expiresIn
  - openUserId
  - appId
  - ea
  - errorCode
  - errorMessage
  - traceId
  token_endpoint: https://open.fxiaoke.com/oauth2.0/token
  token_lifetime_seconds: 7200
  token_query_params:
  - thirdTraceId
  type: oauth2
- authorization_endpoint: https://open.fxiaoke.com/oauth2.0/cli/authorize
  code_challenge_methods:
  - S256
  description: Modern OAuth 2.1 authorization server discoverable via RFC 8414 metadata at https://open.fxiaoke.com/.well-known/oauth-authorization-server. Public clients (token_endpoint_auth_methods = none) use PKCE (S256) with authorization_code and refresh_token grants, and may self-register via the RFC 7591 dynamic client registration endpoint.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://open.fxiaoke.com/oauth2.0
  jwks_uri: https://open.fxiaoke.com/oauth2.0/jwks
  name: oauth2.1-pkce
  registration_endpoint: https://open.fxiaoke.com/oauth2.0/register
  token_endpoint: https://open.fxiaoke.com/oauth2.0/pkce/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: fxiaoke-authentication
source_filename: fxiaoke-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fxiaoke.com/openapi_v2/en/start/auth/app-info.html\ndocs: https://developer.fxiaoke.com/openapi_v2/en/start/quickstart/start.html\nsummary:\n  types: [oauth2, custom-token]\n  api_key_in: [body]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  base_host: https://open.fxiaoke.com\nschemes:\n- name: enterprise-app-token\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Self-built enterprise application flow. A tenant creates a self-built app in the\n    Fxiaoke admin console (developer mode) and receives appId, appSecret, and a\n    permanentCode. These are exchanged for a short-lived access token (called\n    corpAccessToken / app access token) that authenticates all subsequent Open API v2\n    calls.\n  token_endpoint: https://open.fxiaoke.com/oauth2.0/token\n  token_query_params:\n  - thirdTraceId   # caller-supplied random trace string\n  request:\n    content_type: application/json\n\
  \    method: POST\n    fields:\n    - {name: appId, required: true}\n    - {name: appSecret, required: true}\n    - {name: permanentCode, required: true}\n    - {name: grantType, required: true, value: app_secret}\n  response_fields:\n  - accessToken\n  - expiresIn\n  - openUserId\n  - appId\n  - ea            # enterprise account\n  - errorCode\n  - errorMessage\n  - traceId\n  token_lifetime_seconds: 7200\n  caching_guidance: >-\n    Token is valid for 2 hours (7200s). Callers must cache it for at least 6600s and\n    refresh by re-calling the token endpoint between 6650s and 7200s; the token\n    expires at 7200s.\n- name: oauth2.1-pkce\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Modern OAuth 2.1 authorization server discoverable via RFC 8414 metadata at\n    https://open.fxiaoke.com/.well-known/oauth-authorization-server. Public clients\n    (token_endpoint_auth_methods = none) use PKCE (S256) with authorization_code and\n    refresh_token grants, and may self-register\
  \ via the RFC 7591 dynamic client\n    registration endpoint.\n  issuer: https://open.fxiaoke.com/oauth2.0\n  authorization_endpoint: https://open.fxiaoke.com/oauth2.0/cli/authorize\n  token_endpoint: https://open.fxiaoke.com/oauth2.0/pkce/token\n  registration_endpoint: https://open.fxiaoke.com/oauth2.0/register\n  jwks_uri: https://open.fxiaoke.com/oauth2.0/jwks\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  id_token_signing_alg: [RS256]\nnotes: >-\n  Open API v2 calls carry the token plus tenant context (corpId / currentOpenUserId\n  derived from openUserId) in the JSON request body rather than an Authorization\n  header. No OpenAPI/Swagger definition is published, so this profile was captured\n  from the developer documentation and the live RFC 8414 metadata rather than derived\n  from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxiaoke/refs/heads/main/authentication/fxiaoke-authentication.yml
summary_line: oauth2/custom-token · 2 schemes
tags:
- Company
- Enterprise
- CRM
- Sales
- Marketing
- Customer Service
- SaaS
- China
- PaaS
---
