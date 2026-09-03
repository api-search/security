---
api_key_in: []
api_specs:
- filename: upstox-developer-api-openapi.yml
  format: yaml
  label: Upstox Developer API
  slug: upstox-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/openapi/upstox-developer-api-openapi.yml
auth_types:
- oauth2
description: 'Upstox authenticates every API call with an OAuth 2.0 bearer token issued through the authorization code flow. All logins happen on upstox.com — there is deliberately no endpoint that lets a third-party app collect a customer''s Upstox credentials — so an integrator redirects the customer to Upstox, receives a single-use authorization code on a pre-registered redirect URI, and exchanges it server-to-server for an access token. The operational wrinkle that shapes every automated integration is token lifetime: a standard access token lasts one trading day, so Upstox publishes three separate ways to get one (interactive, semi-automated via a notifier webhook, and manual from the dashboard) plus a long-lived read-only Analytics Token that trades daily re-auth for a registered static IP.'
kind: authentication
layout: security
method: searched
name: Upstox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Upstox secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Upstox
provider_slug: upstox
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api-v2.upstox.com/v2/login/authorization/dialog
    documented_authorizationUrl: https://api.upstox.com/v2/login/authorization/dialog
    documented_tokenUrl: https://api.upstox.com/v2/login/authorization/token
    flow: authorizationCode
    note: The served OpenAPI declares the api-v2.upstox.com spelling of both endpoints while the authentication documentation uses api.upstox.com. Both resolve; the documented form is the one to code against.
    pkce: false
    refresh_token: false
    scopes: 2
    tokenUrl: https://api-v2.upstox.com/v2/login/authorization/token
    token_endpoint_content_type: application/x-www-form-urlencoded
  format: Bearer <access_token>
  header: Authorization
  in: header
  name: OAUTH2
  sources:
  - openapi/upstox-developer-api-openapi.yml
  - https://upstox.com/developer/api-documentation/authentication
  type: oauth2
slug: upstox-authentication
source_filename: upstox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://upstox.com/developer/api-documentation/authentication,\n  https://upstox.com/developer/api-documentation/analytics-token,\n  https://upstox.com/developer/api-documentation/access-token-request and\n  openapi/upstox-developer-api-openapi.yml (derived baseline upgraded with the docs)\ndocs: https://upstox.com/developer/api-documentation/authentication\nname: Upstox API authentication\ndescription: >-\n  Upstox authenticates every API call with an OAuth 2.0 bearer token issued through the authorization\n  code flow. All logins happen on upstox.com — there is deliberately no endpoint that lets a third-party\n  app collect a customer's Upstox credentials — so an integrator redirects the customer to Upstox,\n  receives a single-use authorization code on a pre-registered redirect URI, and exchanges it\n  server-to-server for an access token. The operational wrinkle that shapes every automated integration\n  is token\
  \ lifetime: a standard access token lasts one trading day, so Upstox publishes three separate\n  ways to get one (interactive, semi-automated via a notifier webhook, and manual from the dashboard)\n  plus a long-lived read-only Analytics Token that trades daily re-auth for a registered static IP.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  scheme_count: 1\n  applied_to_operations: 101\nschemes:\n- name: OAUTH2\n  type: oauth2\n  in: header\n  header: Authorization\n  format: Bearer <access_token>\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-v2.upstox.com/v2/login/authorization/dialog\n    documented_authorizationUrl: https://api.upstox.com/v2/login/authorization/dialog\n    tokenUrl: https://api-v2.upstox.com/v2/login/authorization/token\n    documented_tokenUrl: https://api.upstox.com/v2/login/authorization/token\n    token_endpoint_content_type: application/x-www-form-urlencoded\n    scopes: 2\n    pkce: false\n    refresh_token:\
  \ false\n    note: >-\n      The served OpenAPI declares the api-v2.upstox.com spelling of both endpoints while the\n      authentication documentation uses api.upstox.com. Both resolve; the documented form is the one to\n      code against.\n  sources:\n  - openapi/upstox-developer-api-openapi.yml\n  - https://upstox.com/developer/api-documentation/authentication\nauthorization_request:\n  endpoint: https://api.upstox.com/v2/login/authorization/dialog\n  operationId: authorize\n  parameters:\n  - name: client_id\n    required: true\n    description: The API key from app creation. In OAuth terms this is the API Key, not the customer's UCC.\n  - name: redirect_uri\n    required: true\n    description: Must exactly match the redirect URI registered during app creation.\n  - name: response_type\n    required: true\n    description: Must always be `code`.\n  - name: state\n    required: false\n    description: Returned unchanged on the callback for request/response continuity.\n  gotchas:\n\
  \  - Redirect URLs ending in .php or similar extensions may be blocked; Upstox advises not placing the redirect at the end of the URL.\n  - An Invalid Credentials error (UDAPI100016) usually means client_id, redirect_uri or response_type does not match the registered app values.\ntoken_exchange:\n  endpoint: https://api.upstox.com/v2/login/authorization/token\n  operationId: token\n  method: POST\n  server_to_server: true\n  content_type: application/x-www-form-urlencoded\n  parameters:\n  - code\n  - client_id\n  - client_secret\n  - redirect_uri\n  - grant_type\n  grant_type: authorization_code\n  code_single_use: true\n  code_note: The authorization code is valid for a single use regardless of whether token generation succeeds.\ntoken_types:\n- name: access_token\n  lifetime: one trading day\n  scope: full API surface subject to app permissions\n  renewal: Re-run the authorization code flow, or use the semi-automated or manual paths.\n- name: extended_token\n  lifetime: extended\n \
  \ restriction: >-\n    Not permitted on every API. Calling a disallowed endpoint returns UDAPI100067 — \"The API you are\n    trying to access is not permitted with an extended_token\".\n- name: Analytics Token\n  lifetime: 1 year\n  access: read-only\n  scope: >-\n    Market data freely; portfolio, positions, holdings, orders and profit-and-loss require the account to\n    have a registered static IP.\n  docs: https://upstox.com/developer/api-documentation/analytics-token\n  announced: '2026-03-20'\n- name: sandbox access token\n  lifetime: 30 days\n  scope: sandbox orders only; cannot be used for live transactions\n  docs: https://upstox.com/developer/api-documentation/sandbox\ntoken_acquisition_methods:\n- method: authorization code flow\n  best_for: Apps that log customers in interactively.\n  delivery: Exchanged on your server from a single-use code.\n- method: semi-automated\n  best_for: Scheduled or automated apps that still require human approval.\n  delivery: >-\n    The app triggers\
  \ an auth request at a scheduled time; the customer approves from a mobile\n    notification or the Developer Apps page, and the token is pushed to the app's notifier URL.\n  docs: https://upstox.com/developer/api-documentation/access-token-request\n  status: beta\n- method: manual\n  best_for: One-off or personal utilities.\n  delivery: Generated and copied from the developer dashboard at https://account.upstox.com/developer/apps.\ncustomer_authentication:\n  location: upstox.com only\n  note: >-\n    There is no public endpoint that lets another application log a customer into upstox.com. Upstox\n    states all logins and logouts are handled exclusively by upstox.com for security and compliance.\n  mfa:\n    supported: true\n    factors:\n    - PIN (1FA)\n    - SMS OTP (2FA)\n    - TOTP (2FA, opt-in alternative to SMS OTP)\nsession_termination:\n  operationId: logout\n  endpoint: DELETE /v2/logout\n  effect: Invalidates the active access token and ends the session.\nstatic_ip:\n  required_for:\n\
  \  - Algo trading order flow (per the exchange circular dated 5 May 2025)\n  - Account-scoped APIs when using the Analytics Token\n  management_operations:\n  - getUserIps\n  - updateUserIp\n  limits: Weekly update limits apply; a successful update invalidates the current token.\n  docs: https://upstox.com/developer/api-documentation/update-app-static-ips\nmcp_authentication:\n  server: https://mcp.upstox.com/mcp\n  model: OAuth 2.0 with dynamic client registration and PKCE (S256), separate from the REST authorization server.\n  reauthorization: daily\n  detail: mcp/upstox-mcp.yml\n  metadata: well-known/upstox-mcp-oauth-authorization-server.json\ngaps:\n- No PKCE on the REST authorization code flow (only the MCP authorization server advertises it).\n- No refresh_token grant on the REST flow — the daily expiry must be re-authorized, which is why the semi-automated and Analytics Token paths exist.\n- Only 32 of 101 operations declare a 401 response in the OpenAPI despite the whole surface\
  \ being OAuth protected.\n- No /.well-known/openid-configuration and no OpenID Connect scheme; Upstox is an OAuth authorization provider, not an identity provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/authentication/upstox-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Financial Services
- Stock Trading
- Brokerage
- Market Data
- Investing
- Capital Markets
- Mutual Funds
- Algorithmic Trading
- India
---
