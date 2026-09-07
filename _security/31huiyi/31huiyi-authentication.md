---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 31huiyi-openapi.postman_collection.json
  format: json
  label: 31 OpenAPI
  slug: 31huiyi-openapi
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/postman/31huiyi-openapi.postman_collection.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: 31Huiyi Authentication
name_suffix: Authentication
oauth_flows: []
overview: 31huiyi declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: 31huiyi
provider_slug: 31huiyi
scheme_count: 4
schemes:
- description: The documented server-to-server flow. POST application/x-www-form-urlencoded to /connect/token with grant_type=custom_user_code, client_id=openapi, method=client_secret, scope="offline_access OpenAppGateway", appKey and appSecret. Returns access_token, expires_in, token_type (Bearer), refresh_token and scope.
  flow: client_credentials
  grant_type: custom_user_code
  id: oauth2_client_credentials
  parameters:
  - documented_default: custom_user_code
    name: grant_type
    required: true
  - documented_default: openapi
    name: client_id
    required: true
  - documented_default: offline_access OpenAppGateway
    name: scope
    required: true
  - documented_default: client_secret
    name: method
    required: true
  - name: appKey
    note: Issued by 31 integration staff.
    required: true
  - name: appSecret
    note: Issued by 31 integration staff.
    required: true
  source: https://api-help.31huiyi.com/zh/home
  token_endpoint: https://oauth.31huiyi.com/connect/token
  type: oauth2
- description: POST grant_type=refresh_token with client_id and refresh_token to mint a new access token.
  flow: refresh_token
  id: oauth2_refresh_token
  source: https://api-help.31huiyi.com/zh/home
  token_endpoint: https://oauth.31huiyi.com/connect/token
  type: oauth2
- applies_to: https://31api.31huiyi.com
  description: 'Business operations carry Authorization: Bearer ${access_token}. Operations published under the /op/notoken/ path prefix are documented as callable without a user token (client authorization still applies); operations under /op/api/ and /op/userresource/ require the Bearer header.'
  id: bearer_token
  scheme: bearer
  source: https://api-help.31huiyi.com/zh/GetAttendeeDetail
  type: http
- description: The authorization server publishes a full OIDC discovery document anonymously, advertising authorization, token, userinfo, endsession, checksession, revocation, introspection and device authorization endpoints, RS256 id_tokens and PKCE (plain and S256).
  id: openid_connect
  openIdConnectUrl: https://oauth.31huiyi.com/.well-known/openid-configuration
  source: https://oauth.31huiyi.com/.well-known/openid-configuration
  type: openIdConnect
slug: 31huiyi-authentication
source_filename: 31huiyi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://api-help.31huiyi.com/zh/home\ndocs:\n- https://api-help.31huiyi.com/zh/home\n- https://api-help.31huiyi.com/zh/oauth\n- https://api-help.31huiyi.com/zh/frontsso\nprobed:\n- url: https://oauth.31huiyi.com/.well-known/openid-configuration\n  status: 200\n- url: https://oauth.31huiyi.com/.well-known/openid-configuration/jwks\n  status: 200\nname: 31huiyi OpenAPI authentication profile\nsummary: >-\n  The 31 OpenAPI is protected by an OAuth 2.0 / OpenID Connect authorization server (IdentityServer)\n  at https://oauth.31huiyi.com. Clients are issued a client id (appKey) and secret (appSecret) by\n  31's integration staff — there is no self-service registration — and exchange them at\n  /connect/token for a Bearer access token that is sent in the Authorization header on business calls.\nschemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: client_credentials\n  token_endpoint: https://oauth.31huiyi.com/connect/token\n\
  \  grant_type: custom_user_code\n  description: >-\n    The documented server-to-server flow. POST application/x-www-form-urlencoded to /connect/token with\n    grant_type=custom_user_code, client_id=openapi, method=client_secret, scope=\"offline_access\n    OpenAppGateway\", appKey and appSecret. Returns access_token, expires_in, token_type (Bearer),\n    refresh_token and scope.\n  parameters:\n  - name: grant_type\n    required: true\n    documented_default: custom_user_code\n  - name: client_id\n    required: true\n    documented_default: openapi\n  - name: scope\n    required: true\n    documented_default: offline_access OpenAppGateway\n  - name: method\n    required: true\n    documented_default: client_secret\n  - name: appKey\n    required: true\n    note: Issued by 31 integration staff.\n  - name: appSecret\n    required: true\n    note: Issued by 31 integration staff.\n  source: https://api-help.31huiyi.com/zh/home\n- id: oauth2_refresh_token\n  type: oauth2\n  flow: refresh_token\n\
  \  token_endpoint: https://oauth.31huiyi.com/connect/token\n  description: >-\n    POST grant_type=refresh_token with client_id and refresh_token to mint a new access token.\n  source: https://api-help.31huiyi.com/zh/home\n- id: bearer_token\n  type: http\n  scheme: bearer\n  description: >-\n    Business operations carry Authorization: Bearer ${access_token}. Operations published under the\n    /op/notoken/ path prefix are documented as callable without a user token (client authorization\n    still applies); operations under /op/api/ and /op/userresource/ require the Bearer header.\n  applies_to: https://31api.31huiyi.com\n  source: https://api-help.31huiyi.com/zh/GetAttendeeDetail\n- id: openid_connect\n  type: openIdConnect\n  openIdConnectUrl: https://oauth.31huiyi.com/.well-known/openid-configuration\n  description: >-\n    The authorization server publishes a full OIDC discovery document anonymously, advertising\n    authorization, token, userinfo, endsession, checksession, revocation,\
  \ introspection and device\n    authorization endpoints, RS256 id_tokens and PKCE (plain and S256).\n  source: https://oauth.31huiyi.com/.well-known/openid-configuration\ntoken:\n  format: JWT Bearer (RS256, per the OIDC discovery id_token_signing_alg_values_supported)\n  access_token_ttl: 30 minutes\n  refresh_token_ttl: 2 hours\n  header: 'Authorization: Bearer ${access_token}'\n  source: https://api-help.31huiyi.com/zh/home\nendpoints:\n  authorization: https://oauth.31huiyi.com/connect/authorize\n  token: https://oauth.31huiyi.com/connect/token\n  userinfo: https://oauth.31huiyi.com/connect/userinfo\n  revocation: https://oauth.31huiyi.com/connect/revocation\n  introspection: https://oauth.31huiyi.com/connect/introspect\n  end_session: https://oauth.31huiyi.com/connect/endsession\n  device_authorization: https://oauth.31huiyi.com/connect/deviceauthorization\n  jwks: https://oauth.31huiyi.com/.well-known/openid-configuration/jwks\ngrant_types_supported:\n- authorization_code\n- client_credentials\n\
  - refresh_token\n- implicit\n- password\n- urn:ietf:params:oauth:grant-type:device_code\n- custom_user_code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\npkce:\n  supported: true\n  code_challenge_methods: [plain, S256]\nsso:\n  description: >-\n    31 documents a partner SSO handshake: create or resolve an account with\n    POST /op/userresource/AccountUser/v1/createForClient to obtain an accountId, exchange it for a login\n    code with GET /op/security/usercode?loginUserId=<accountId>, then redirect the browser to\n    {ConfHost}/home/autoLogin.html?uid=<accountId>&code=<usercode>&returl=<target> which lands the user\n    on the target page with a session token.\n  source: https://api-help.31huiyi.com/zh/oauth\nnotes:\n- Credentials are not self-service — the docs state each client contacts 31's integration staff to be\n  issued a unique client id and secret.\n- No API-key authentication scheme is documented; every documented surface is OAuth\
  \ bearer or an\n  explicitly token-free (/op/notoken/) path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/authentication/31huiyi-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Events
- Event Management
- Conferences
- Exhibitions
- Registration
- Check-In
- Scheduling
- Ticketing
- SaaS
- China
---
