---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Wyze Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Wyze secures its APIs with apiKey, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Wyze
provider_slug: wyze
scheme_count: 5
schemes:
- api: wyze:developer-api
  constraints:
    key_lifetime: 1 year from creation
    keys_per_user: 1
    rate_limited: Wyze documents that the login endpoint is rate limited and instructs callers not to repeatedly call it to obtain tokens; no numeric limit is published
    rotation: to rotate, delete the existing key in the console and create a new one; Wyze emails the account when a key is generated
  description: A personal API Key and API Key ID generated from the Wyze Developer API Console at https://developer-api-console.wyze.com/#/apikey/view. Both are sent as HTTP headers (Keyid, Apikey) on the login request along with a JSON body carrying the account email and a triple-MD5 hashed password. The credential is per-user, not per-app.
  endpoint: https://auth-prod.api.wyze.com/api/user/login
  in: header
  name: WyzeApiKeyPair
  parameter_names:
  - Keyid
  - Apikey
  type: apiKey
- api: wyze:developer-api
  description: The access token returned by the login exchange (prefix observed in Wyze's published example as "lvtx."). Used against the api.wyzecam.com application endpoints.
  name: WyzeAccessToken
  scheme: bearer
  token_lifetime: 2 days
  type: http
- api: wyze:developer-api
  description: The refresh token returned by the login exchange, POSTed to /app/user/refresh_token with the documented app_ver / app_version / phone_id / sc / sv constants ("wyze_developer_api") plus a ts timestamp, to mint a new access token and refresh token pair.
  endpoint: https://api.wyzecam.com/app/user/refresh_token
  name: WyzeRefreshToken
  scheme: bearer
  token_lifetime: 30 days
  type: http
- api: wyze:customer-account-mcp
  description: Shopify customer-accounts OIDC, served from Wyze's own hosts. Backs the storefront login and the customer account MCP server.
  endpoints:
    authorization: https://account.wyze.com/authentication/oauth/authorize
    end_session: https://account.wyze.com/authentication/logout
    jwks: https://account.wyze.com/authentication/.well-known/jwks.json
    token: https://account.wyze.com/authentication/oauth/token
  flows:
  - flow: authorizationCode
    pkce:
    - S256
  - flow: refreshToken
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/58004504738
  name: WyzeCustomerAccountOIDC
  openIdConnectUrl: https://www.wyze.com/.well-known/openid-configuration
  response_types:
  - code
  scopes: scopes/wyze-scopes.yml
  source: well-known/wyze-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- api: wyze:ucp
  description: The Universal Commerce Protocol MCP endpoint at /api/ucp/mcp requires the calling agent to present a resolvable agent profile URI; anonymous JSON-RPC tools/list is rejected with error -32001 invalid_profile_url / "Missing profile uri". The exact header/parameter name is not published by Wyze and was not guessed.
  in: request
  name: WyzeUCPAgentProfile
  observed_status: 422
  type: apiKey
slug: wyze-authentication
source_filename: wyze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: >-\n  https://support.wyze.com/hc/en-us/articles/16129834216731-Creating-an-API-Key and\n  https://www.wyze.com/.well-known/openid-configuration, plus live probes of\n  auth-prod.api.wyze.com and api.wyzecam.com\ndocs: https://support.wyze.com/hc/en-us/articles/16129834216731-Creating-an-API-Key\nnotes: >-\n  Wyze publishes no OpenAPI, so nothing here is derived from a spec - every scheme below\n  is taken from Wyze's own published documentation or from a live, unauthenticated probe.\n  Two entirely separate authentication models exist: (1) the device/cloud API, which uses\n  a personal API Key + Key ID pair exchanged for bearer tokens; and (2) the Shopify-backed\n  storefront customer account, which is a standards-compliant OIDC/OAuth 2.0 authorization\n  code + PKCE surface with a published discovery document.\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode,\
  \ refreshToken, jwt-bearer]\n  mfa: >-\n    Wyze mandates 2-factor authentication for all customer accounts (per\n    https://www.wyze.com/pages/security-trust); the login response carries mfa_options,\n    mfa_details, sms_session_id and email_session_id fields.\n\nschemes:\n- name: WyzeApiKeyPair\n  type: apiKey\n  in: header\n  parameter_names: [Keyid, Apikey]\n  api: wyze:developer-api\n  endpoint: https://auth-prod.api.wyze.com/api/user/login\n  description: >-\n    A personal API Key and API Key ID generated from the Wyze Developer API Console at\n    https://developer-api-console.wyze.com/#/apikey/view. Both are sent as HTTP headers\n    (Keyid, Apikey) on the login request along with a JSON body carrying the account\n    email and a triple-MD5 hashed password. The credential is per-user, not per-app.\n  constraints:\n    keys_per_user: 1\n    key_lifetime: 1 year from creation\n    rotation: >-\n      to rotate, delete the existing key in the console and create a new one; Wyze\
  \ emails\n      the account when a key is generated\n    rate_limited: >-\n      Wyze documents that the login endpoint is rate limited and instructs callers not to\n      repeatedly call it to obtain tokens; no numeric limit is published\n\n- name: WyzeAccessToken\n  type: http\n  scheme: bearer\n  api: wyze:developer-api\n  description: >-\n    The access token returned by the login exchange (prefix observed in Wyze's published\n    example as \"lvtx.\"). Used against the api.wyzecam.com application endpoints.\n  token_lifetime: 2 days\n\n- name: WyzeRefreshToken\n  type: http\n  scheme: bearer\n  api: wyze:developer-api\n  endpoint: https://api.wyzecam.com/app/user/refresh_token\n  description: >-\n    The refresh token returned by the login exchange, POSTed to\n    /app/user/refresh_token with the documented app_ver / app_version / phone_id / sc /\n    sv constants (\"wyze_developer_api\") plus a ts timestamp, to mint a new access token\n    and refresh token pair.\n  token_lifetime:\
  \ 30 days\n\n- name: WyzeCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.wyze.com/.well-known/openid-configuration\n  api: wyze:customer-account-mcp\n  source: well-known/wyze-openid-configuration.json\n  issuer: https://shopify.com/authentication/58004504738\n  description: >-\n    Shopify customer-accounts OIDC, served from Wyze's own hosts. Backs the storefront\n    login and the customer account MCP server.\n  endpoints:\n    authorization: https://account.wyze.com/authentication/oauth/authorize\n    token: https://account.wyze.com/authentication/oauth/token\n    end_session: https://account.wyze.com/authentication/logout\n    jwks: https://account.wyze.com/authentication/.well-known/jwks.json\n  flows:\n  - flow: authorizationCode\n    pkce: [S256]\n  - flow: refreshToken\n  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  response_types: [code]\n  scopes: scopes/wyze-scopes.yml\n\
  \n- name: WyzeUCPAgentProfile\n  type: apiKey\n  in: request\n  api: wyze:ucp\n  description: >-\n    The Universal Commerce Protocol MCP endpoint at /api/ucp/mcp requires the calling\n    agent to present a resolvable agent profile URI; anonymous JSON-RPC tools/list is\n    rejected with error -32001 invalid_profile_url / \"Missing profile uri\". The exact\n    header/parameter name is not published by Wyze and was not guessed.\n  observed_status: 422\n\nunauthenticated_surfaces:\n- surface: https://www.wyze.com/api/mcp\n  note: storefront MCP server; tools/list and catalog/cart tools answer with no credentials\n- surface: https://www.wyze.com/.well-known/ucp\n  note: UCP merchant discovery document, public\n- surface: https://www.wyze.com/llms.txt\n  note: agent instructions, public\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyze/refs/heads/main/authentication/wyze-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Smart Home
- Internet of Things
- Home Security
- Cameras
- Consumer Electronics
- Home Automation
- Video
- Sensors
- Commerce
---
