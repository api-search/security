---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Gojek Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: GoJek secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: GoJek
provider_slug: gojek
scheme_count: 2
schemes:
- audience: Merchants integrating their own systems (machine-to-machine)
  client_authentication: HTTP Basic (client_id:client_secret) on the token endpoint
  flow: clientCredentials
  integration_model: Direct Integration
  name: go_auth_client_credentials
  parameters:
  - name: client_id
    required: true
  - name: client_secret
    required: true
  - name: grant_type
    required: true
    value: client_credentials
  - name: scope
    note: If access level is not provided, no scope is granted to the token.
    required: true
  response:
    access_token: string
    expires_in: 3600
    scope: string
    token_type: Bearer
  scope_count: 18
  source: https://developer.gobiz.com/docs/api/auth/direct-integration/
  token_url_production: https://accounts.go-jek.com/oauth2/token
  token_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/token
  type: oauth2
- audience: POS providers and online-order aggregators acting on behalf of merchants
  authorization_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/auth
  flow: authorizationCode
  integration_model: Facilitator
  name: go_auth_authorization_code
  openid_connect: true
  parameters:
  - name: client_id
    required: true
  - name: response_type
    required: true
    value: code
  - name: scope
    note: must include at least 'openid'
    required: true
  - name: state
    note: CSRF token, >= 8 chars, URL-safe encoded (RFC 6749 s10.12)
    required: true
  - name: redirect_uri
    note: must match a redirect URI registered with the client credentials
    required: true
  - name: nonce
    note: binds the client session to the ID Token, mitigates replay
    required: false
  - name: max_age
    required: false
  - name: ui_locales
    note: id | en
    required: false
  returns:
  - access_token
  - id_token (JWT with end-user claims)
  - refresh via the 'offline' scope
  source: https://developer.gobiz.com/docs/api/auth/facilitator/
  standards_cited_by_provider:
  - RFC 6749 (OAuth 2.0)
  - RFC 6819 (OAuth 2.0 Threat Model)
  - OpenID Connect Core 1.0 incorporating errata set 1
  token_url_production: https://accounts.go-jek.com/oauth2/token
  token_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/token
  type: oauth2
slug: gojek-authentication
source_filename: gojek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://developer.gobiz.com/docs/api/auth/direct-integration/\ndocs: https://developer.gobiz.com/docs/category/authentication\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\n  note: >-\n    GoBiz has no API-key surface. Every call to api.gobiz.co.id carries an\n    OAuth 2.0 Bearer token issued by the Gojek GoAuth server. Two integration\n    models exist and each uses a different grant.\nschemes:\n- name: go_auth_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  integration_model: Direct Integration\n  audience: Merchants integrating their own systems (machine-to-machine)\n  token_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/token\n  token_url_production: https://accounts.go-jek.com/oauth2/token\n  client_authentication: HTTP Basic (client_id:client_secret) on the token endpoint\n  parameters:\n  - {name: client_id, required:\
  \ true}\n  - {name: client_secret, required: true}\n  - {name: grant_type, required: true, value: client_credentials}\n  - {name: scope, required: true, note: \"If access level is not provided, no scope is granted to the token.\"}\n  response:\n    access_token: string\n    expires_in: 3600\n    token_type: Bearer\n    scope: string\n  scope_count: 18\n  source: https://developer.gobiz.com/docs/api/auth/direct-integration/\n- name: go_auth_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  openid_connect: true\n  integration_model: Facilitator\n  audience: POS providers and online-order aggregators acting on behalf of merchants\n  authorization_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/auth\n  token_url_sandbox: https://integration-goauth.gojekapi.com/oauth2/token\n  token_url_production: https://accounts.go-jek.com/oauth2/token\n  parameters:\n  - {name: client_id, required: true}\n  - {name: response_type, required: true, value: code}\n  - {name: scope,\
  \ required: true, note: \"must include at least 'openid'\"}\n  - {name: state, required: true, note: \"CSRF token, >= 8 chars, URL-safe encoded (RFC 6749 s10.12)\"}\n  - {name: redirect_uri, required: true, note: \"must match a redirect URI registered with the client credentials\"}\n  - {name: nonce, required: false, note: \"binds the client session to the ID Token, mitigates replay\"}\n  - {name: max_age, required: false}\n  - {name: ui_locales, required: false, note: \"id | en\"}\n  returns:\n  - access_token\n  - id_token (JWT with end-user claims)\n  - refresh via the 'offline' scope\n  standards_cited_by_provider:\n  - RFC 6749 (OAuth 2.0)\n  - RFC 6819 (OAuth 2.0 Threat Model)\n  - OpenID Connect Core 1.0 incorporating errata set 1\n  source: https://developer.gobiz.com/docs/api/auth/facilitator/\nrequest_header:\n  name: Authorization\n  value: \"Bearer {access-token}\"\n  required: true\nwebhook_authentication:\n  header: X-Go-Signature\n  algorithm: HMAC-SHA256(notification_secret_key,\
  \ request_body)\n  source: https://developer.gobiz.com/docs/api/webhooks/receiving-notifications/\ndiscovery:\n  openid_configuration: not published (probed 2026-08-22, 404 on accounts.go-jek.com and integration-goauth.gojekapi.com)\n  oauth_authorization_server: not published (probed 2026-08-22, 404)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojek/refs/heads/main/authentication/gojek-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Super App
- Ride Hailing
- Food Delivery
- Point of Sale
- Merchant Platform
- Payments
- QRIS
- Logistics
- Indonesia
- Southeast Asia
- Webhooks
- OAuth
---
