---
api_key_in:
- header
api_specs:
- filename: ci-hub-access-openapi.yml
  format: yaml
  label: CI HUB Access SDK API
  slug: access-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/openapi/ci-hub-access-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ci Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: CI HUB secures its APIs with http, apiKey, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CI HUB
provider_slug: ci-hub
scheme_count: 0
schemes: []
slug: ci-hub-authentication
source_filename: ci-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developer.ci-hub.com/access/authentication\nderived_from: openapi/ci-hub-access-openapi.yml\nnote: >-\n  CI HUB runs two entirely different authentication models side by side, and a partner touching\n  both surfaces has to implement both. The Access SDK uses a proprietary partner-JWT token\n  exchange with a second, per-DAM token layered on top — no OAuth, no scopes, no authorization\n  endpoint. The MCP server uses standards-compliant OAuth 2.1 with discovery metadata and dynamic\n  client registration. Neither is wrong; they just are not the same system, and nothing in the\n  docs connects them.\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  models: 2\n  scopes: 1\n  mfa_or_user_consent_step: true\nmodels:\n- id: access-sdk\n  applies_to: ci-hub:access-sdk\n  style: two-token — partner JWT exchange, plus a per-DAM connection token\n  standard: none (JWT/JWKS building blocks, but\
  \ not OAuth 2.0 or RFC 7523)\n  docs: https://developer.ci-hub.com/access/authentication\n  bootstrap:\n    step: POST /auth/exchangeToken\n    operation: exchangeToken\n    presented_credential: partner-signed JWT in Authorization Bearer\n    algorithm: RS256 (HS256 explicitly rejected)\n    root_of_trust: >-\n      the partner's published JWKS URL, registered with CI HUB at onboarding and cached by CI HUB\n      for 10 minutes; the JWT `kid` must match a key in that set\n    required_claims:\n    - iss — the registered partner issuer, matched exactly including any trailing slash\n    - aud — the registered audience, default https://api.ci-hub.com\n    - sub — stable identifier for the user in the partner system\n    - iat — unix seconds; up to 30s future tolerance; rejected once older than maxTokenAge\n    - exp — unix seconds, must be in the future\n    - email — required in the JWT or the JSON request body; drives JIT user resolution\n    optional_claims:\n    - given_name\n    - family_name\n\
  \    - name\n    max_token_age: 3600 seconds by default, measured from iat\n    single_use: the partner JWT is consumed once per exchange and discarded\n    trap: >-\n      `aud` is always https://api.ci-hub.com on EVERY environment. It identifies CI HUB in the\n      partner registration and does not change with the client's baseUrl. Setting it to the host\n      you are calling returns 403 cihub-sdk-audience-invalid.\n  schemes:\n  - name: cihubAccessToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: Authorization\n    algorithm: HS256\n    lifetime: 1 hour\n    required_on: every call after the exchange\n    description: >-\n      CI HUB access token returned by POST /auth/exchangeToken. Identifies the user inside CI HUB.\n      On POST /auth/exchangeToken itself this header instead carries the partner-signed RS256 JWT.\n    sources:\n    - openapi/ci-hub-access-openapi.yml\n  - name: damToken\n    type: apiKey\n    in: header\n    parameter: provider-authorization\n\
  \    format: Bearer <DAM connection token>\n    lifetime: provider-dependent; not reported at login\n    required_on: >-\n      calls that reach a specific DAM — folder browse, search, asset detail, versions, download,\n      thumbnail\n    description: >-\n      DAM connection token obtained from the provider login flow. Authorizes access to the DAM\n      itself, which authenticates separately from CI HUB. The partner platform obtains and stores\n      these; CI HUB does not persist them server-side.\n    overload_warning: >-\n      On GET /auth/refreshToken this same header carries the CI HUB REFRESH token rather than a DAM\n      token, and the refresh token's sub must match the access token's sub. It is the one place the\n      two-token rule does not hold.\n    sources:\n    - openapi/ci-hub-access-openapi.yml\n  token_lifetimes:\n  - token: partner JWT\n    lifetime: up to maxTokenAge (1 hour default)\n    algorithm: RS256\n    storage: minted per exchange, discarded\n  - token:\
  \ CI HUB access token\n    lifetime: 1 hour\n    algorithm: HS256\n    storage: cached by the partner, sent on every call\n  - token: CI HUB refresh token\n    lifetime: 30 days\n    algorithm: HS256\n    storage: cached by the partner, used to mint new access tokens\n  - token: DAM connection token\n    lifetime: provider-dependent, not reported\n    storage: held by the partner platform; not persisted by CI HUB\n  refresh:\n    operation: refreshTokenSdk\n    endpoint: GET /auth/refreshToken\n    behavior: >-\n      Mints a new access token AND a new refresh token. The previous access token is superseded but\n      remains valid until its exp; the previous refresh token remains valid for its full 30 days,\n      so a slow client switch-over is safe. Refresh the CI HUB session proactively from expires_in;\n      refresh a DAM session reactively on the first 401, since providers report no lifetime.\n  dam_login:\n    operations:\n    - damLoginInitiate\n    - damLoginPoll\n    style: browser\
  \ redirect at the DAM plus server-side polling on a one-time `state`\n    note: >-\n      Most DAMs use OAuth on their own side, so the redirect is part of the DAM's flow, not CI\n      HUB's. The CI HUB token exchange itself has no browser redirect at all.\n    provider_params:\n      serverUrl: >-\n        the DAM instance origin, read by bynder, dash, fotoware, frontify, picturepark and purered;\n        supplying it removes the instance-prompt page from the user's flow\n  session_end:\n    operation: logoutSdk\n    endpoint: GET /auth/logout\n  validation:\n    operation: checkTokenSdk\n    endpoint: GET /auth/checkToken\n    returns: >-\n      the user profile envelope plus licenseState, licenseExpires and isTrialLicense describing the\n      SDK subscription. A 401 means start a new exchange; a 402 means the subscription state\n      changed and is an operational, not technical, problem.\n- id: mcp\n  applies_to: ci-hub:mcp\n  style: OAuth 2.1 authorization code with PKCE\n  standard:\
  \ OAuth 2.1, RFC 8414, RFC 9728, RFC 7591, RFC 7636\n  resource: https://mcp.ci-hub.com\n  authorization_server: https://mcp-auth.ci-hub.com\n  discovery:\n  - https://mcp.ci-hub.com/.well-known/oauth-protected-resource\n  - https://mcp-auth.ci-hub.com/.well-known/oauth-authorization-server\n  - https://mcp-auth.ci-hub.com/.well-known/openid-configuration\n  challenge: >-\n    WWW-Authenticate: Bearer error=\"unauthorized\", error_description=\"Authorization needed\",\n    resource_metadata=\"https://mcp.ci-hub.com/.well-known/oauth-protected-resource\"\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce: S256 only\n  dynamic_client_registration: true\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  scopes:\n  - cihub\n  second_factor: >-\n    The OAuth grant is only half the authorization. Each end user separately authenticates the DAM\n    accounts they want reachable, and CI HUB maps that user's existing DAM permissions onto\
  \ every\n    tool call. Users change what is reachable by disconnecting and reconnecting.\n  see: scopes/ci-hub-scopes.yml\nauthorization_model:\n  cihub_layer: identity only — the CI HUB token says who the user is, not what they may touch\n  dam_layer: >-\n    every permission decision is the DAM's. integration-forbidden (403) forwards a DAM permission\n    denial verbatim, and the docs are explicit that \"permission decisions are governed by the DAM\".\n  consequence: >-\n    There is no CI HUB-side permission surface to inspect, grant or revoke. An auditor asking what\n    a CI HUB token can reach has to ask each connected DAM instead.\nx-evidence:\n  fetched: '2026-08-12'\n  checks:\n  - url: https://developer.ci-hub.com/access/authentication\n    http_status: 200\n  - url: https://live.ci-hub.com/api/v1/system/providerInfo\n    http_status: 401\n    note: 'anonymous call returns errorCode cihub-access-token-missing, confirming the Authorization\n      requirement'\n  - url: https://mcp.ci-hub.com/.well-known/oauth-protected-resource\n\
  \    http_status: 200\n  - url: https://mcp-auth.ci-hub.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/authentication/ci-hub-authentication.yml
summary_line: http/apiKey/oauth2 · 0 schemes
tags:
- Company
- Digital Asset Management
- Content Management
- Product Information Management
- Integration
- Connectors
- Creative Tools
- Marketing
- Brand Management
- MCP
- Cloud Storage
- Germany
---
