---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Altruist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Altruist secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Altruist
provider_slug: altruist
scheme_count: 2
schemes:
- access_token_ttl_seconds: 3600
  api: Altruist Open API
  authorizationUrl: https://oauth.stage1.altruistnet.tech/api/oauth2/authorize
  credential_header: 'Authorization: <access_token>'
  flow: authorizationCode
  name: OpenAPI-OAuth2-AuthorizationCode
  parameters:
    authorize:
    - client_id
    - redirect_uri
    - scope
    - state
    token:
    - client_id
    - client_secret
    - code
    - refresh_token
    - grant_type
    - token_type
  redirect_uri_rules: HTTPS required; localhost not supported; must be whitelisted
  refresh_token_ttl_days: 30
  scopes:
  - openid
  source: https://developer.altruist.com/docs/open-api-authentication
  tokenUrl: https://openapi.altruist.com/altruist-open-api/oauth2/token
  type: oauth2
- access_token_ttl_seconds: 300
  api: Altruist Realtime API
  credential_header: 'Authorization: Bearer <access_token>'
  flow: password
  identity_provider: Keycloak / OpenID Connect (realm "altruist")
  name: Realtime-OAuth2-Password
  parameters:
    token:
    - grant_type
    - username
    - password
    - client_id
    - client_secret
  sandbox_tokenUrl: https://auth.demo1.altruistnet.tech/realms/altruist/protocol/openid-connect/token
  source: https://developer.altruist.com/docs/authentication-1
  tokenUrl: https://auth.altruist.com/realms/altruist/protocol/openid-connect/token
  type: oauth2
slug: altruist-authentication
source_filename: altruist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.altruist.com/docs/open-api-authentication\ndocs:\n- https://developer.altruist.com/docs/open-api-authentication\n- https://developer.altruist.com/docs/authentication-1\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, password]\n  notes: >-\n    Altruist exposes two API surfaces, each with its own OAuth 2.0 model. The\n    Open API uses the OAuth 2.0 Authorization Code flow (partner-facing,\n    consent-based). The Realtime API uses the OAuth 2.0 Resource Owner Password\n    Credentials grant against a Keycloak/OpenID Connect realm. Both present the\n    access token as an `Authorization: Bearer <token>` header. No API-key auth.\nschemes:\n- name: OpenAPI-OAuth2-AuthorizationCode\n  api: Altruist Open API\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://oauth.stage1.altruistnet.tech/api/oauth2/authorize\n  tokenUrl: https://openapi.altruist.com/altruist-open-api/oauth2/token\n\
  \  scopes: [openid]\n  credential_header: 'Authorization: <access_token>'\n  parameters:\n    authorize: [client_id, redirect_uri, scope, state]\n    token: [client_id, client_secret, code, refresh_token, grant_type, token_type]\n  redirect_uri_rules: HTTPS required; localhost not supported; must be whitelisted\n  access_token_ttl_seconds: 3600\n  refresh_token_ttl_days: 30\n  source: https://developer.altruist.com/docs/open-api-authentication\n- name: Realtime-OAuth2-Password\n  api: Altruist Realtime API\n  type: oauth2\n  flow: password\n  tokenUrl: https://auth.altruist.com/realms/altruist/protocol/openid-connect/token\n  sandbox_tokenUrl: https://auth.demo1.altruistnet.tech/realms/altruist/protocol/openid-connect/token\n  credential_header: 'Authorization: Bearer <access_token>'\n  parameters:\n    token: [grant_type, username, password, client_id, client_secret]\n  access_token_ttl_seconds: 300\n  identity_provider: Keycloak / OpenID Connect (realm \"altruist\")\n  source: https://developer.altruist.com/docs/authentication-1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruist/refs/heads/main/authentication/altruist-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Custody
- Wealth Management
- Financial Advisors
- RIA
- Investing
- OAuth
---
