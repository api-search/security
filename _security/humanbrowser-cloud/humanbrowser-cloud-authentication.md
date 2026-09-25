---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: humanbrowser-cloud-openapi.json
  format: json
  label: Human Browser API
  slug: human-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/openapi/humanbrowser-cloud-openapi.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Humanbrowser Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials (declared in the OpenAPI; tokenUrl dead)
- authorizationCode + PKCE (live on agent.humanbrowser.cloud via RFC 8414 metadata; undocumented)
overview: Virix Labs secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials (declared in the OpenAPI; tokenUrl dead) and authorizationCode + PKCE (live on agent.humanbrowser.cloud via RFC 8414 metadata; undocumented) flow(s).
provider_name: Virix Labs
provider_slug: humanbrowser-cloud
scheme_count: 4
schemes:
- description: 'Human Browser API token (hb_live_… or trial). Send as Authorization: Bearer <token>.'
  issuance:
    dashboard: https://humanbrowser.cloud/account
    paid: issued on first top-up; the card says POST /api/buy returns a fresh token by webhook after a crypto payment
    trial: POST /api/trial-balance {email} (claimTrial) — $10 balance, one per email, revoked after 14 days without a top-up
  name: bearerAuth
  observed:
  - body: '{"error":"unauthorized","hint":"Authorization: Bearer hb_live_<token>"}'
    status: 401
    url: POST https://agent.humanbrowser.cloud/mcp
    www_authenticate: Bearer realm="humanbrowser-mcp"
  - body: 'JSON-RPC error -32001 Unauthorized, data.hint "Authorization: Bearer <token>"'
    status: 401
    url: POST https://agent.humanbrowser.cloud/a2a
  - body: '{"error":"Unauthorized. Pass Authorization: Bearer <DEPLOY_SECRET>"}'
    note: the live route asks for a deployment secret, not a customer token
    status: 401
    url: GET https://humanbrowser.cloud/api/usage
  rules:
  - never put the token in a URL query string (agent card)
  - the MCP endpoint refuses non-Bearer auth
  - tokens are hashed at rest (Privacy 10)
  - report a suspected compromise by email (Terms 3)
  scheme: bearer
  sources:
  - openapi/humanbrowser-cloud-openapi.json
  - https://humanbrowser.cloud/docs/mcp
  token_prefix: hb_live_
  type: http
  used_by:
  - topUp
  - getUsage
  - runA2ATask
  - POST /mcp (hosted MCP)
  - GET /api/balance on the agent host (CLI balance; not in the OpenAPI)
- description: Login session cookie for account endpoints.
  in: cookie
  name: sessionCookie
  observed:
  - body: '{"error":"bad-token"}'
    note: without a cookie or token
    status: 400
    url: GET https://humanbrowser.cloud/api/account
  parameter: hb_session
  sources:
  - openapi/humanbrowser-cloud-openapi.json
  type: apiKey
  used_by:
  - getAccount
- description: Least-privilege scoped access. Request only the scopes an agent needs.
  flows:
  - flow: clientCredentials
    scope_list:
    - session:run
    - account:read
    - account:topup
    scopes: 3
    tokenUrl: https://agent.humanbrowser.cloud/oauth/token
  name: oauth2
  observed:
  - method: GET
    status: 404
    url: https://agent.humanbrowser.cloud/oauth/token
  - body: '{"error":"not-found","path":"/oauth/token"}'
    method: POST
    status: 404
    url: https://agent.humanbrowser.cloud/oauth/token
  sources:
  - openapi/humanbrowser-cloud-openapi.json
  status: declared but not reachable
  type: oauth2
  used_by:
  - getAccount (account:read)
  - topUp (account:topup)
  - getUsage (account:read)
  - runA2ATask (session:run)
- description: The OAuth 2.1 door an MCP client following RFC 9728 discovery would find; scopes and endpoints from the two well-known documents. No human-readable documentation exists for it.
  flows:
  - authorizationUrl: https://agent.humanbrowser.cloud/authorize
    client_auth:
    - none
    - client_secret_post
    client_ids: CIMD URL (https://) or DCR id hbc_<32hex>
    flow: authorizationCode
    pkce: S256 required (only method listed)
    refreshUrl: https://agent.humanbrowser.cloud/token
    registrationUrl: https://agent.humanbrowser.cloud/register
    revocationUrl: https://agent.humanbrowser.cloud/revoke
    scopes:
    - mcp:run
    - mcp:read
    tokenUrl: https://agent.humanbrowser.cloud/token
  name: mcp-oauth (RFC 8414 / RFC 9728, not in the OpenAPI)
  observed:
  - body: unsupported_response_type — response_type must be code
    status: 400
    url: GET /authorize
  - body: invalid_client — client_id must be CIMD URL (https://) or DCR id (hbc_<32hex>)
    status: 400
    url: GET /authorize?response_type=code&client_id=probe
  - body: unsupported_grant_type — grant_type must be authorization_code or refresh_token
    status: 400
    url: POST /token (empty form)
  - status: 404
    url: GET /token
  - note: POST not attempted (would register a client)
    status: 404
    url: GET /register
  - status: 404
    url: https://humanbrowser.cloud/docs/oauth (service_documentation)
  resource: https://agent.humanbrowser.cloud/mcp
  sources:
  - well-known/humanbrowser-cloud-oauth-authorization-server.json
  - well-known/humanbrowser-cloud-oauth-protected-resource.json
  status: live but undocumented
  type: oauth2
slug: humanbrowser-cloud-authentication
source_filename: humanbrowser-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/humanbrowser-cloud-openapi.json\ndocs:\n- https://humanbrowser.cloud/docs/mcp\n- https://humanbrowser.cloud/a2a\n- https://agent.humanbrowser.cloud/.well-known/oauth-authorization-server\n- https://agent.humanbrowser.cloud/.well-known/oauth-protected-resource\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - clientCredentials (declared in the OpenAPI; tokenUrl dead)\n  - authorizationCode + PKCE (live on agent.humanbrowser.cloud via RFC 8414 metadata; undocumented)\n  bearer: true\n  credential_classes: 4\n  headline: >-\n    One prepaid-balance bearer token (hb_live_...) is the credential every published integration uses —\n    the A2A endpoint, the hosted MCP endpoint, the stdio MCP server (HB_TOKEN env, legacy alias\n    HUMANBROWSER_API_TOKEN), the SDK, the CLI and the token-scoped REST operations. A dashboard session\n    cookie (hb_session) guards getAccount.\
  \ The OpenAPI also declares an oauth2 clientCredentials scheme\n    with three scopes whose tokenUrl 404s, and the agent host serves a live OAuth 2.1 authorization server\n    (authorization code + PKCE S256, client-ID metadata documents or DCR ids hbc_<32hex>, scopes mcp:run /\n    mcp:read) advertised for the MCP resource by RFC 9728 metadata — but no documentation page describes\n    that flow (service_documentation /docs/oauth 404) and every guide says \"use the bearer token\".\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  token_prefix: hb_live_\n  description: 'Human Browser API token (hb_live_… or trial). Send as Authorization: Bearer <token>.'\n  issuance:\n    trial: POST /api/trial-balance {email} (claimTrial) — $10 balance, one per email, revoked after 14 days without a top-up\n    paid: issued on first top-up; the card says POST /api/buy returns a fresh token by webhook after a crypto payment\n    dashboard: https://humanbrowser.cloud/account\n  used_by: [topUp,\
  \ getUsage, runA2ATask, 'POST /mcp (hosted MCP)', 'GET /api/balance on the agent host (CLI balance; not in the OpenAPI)']\n  observed:\n  - {url: 'POST https://agent.humanbrowser.cloud/mcp', status: 401, www_authenticate: 'Bearer realm=\"humanbrowser-mcp\"', body: '{\"error\":\"unauthorized\",\"hint\":\"Authorization: Bearer hb_live_<token>\"}'}\n  - {url: 'POST https://agent.humanbrowser.cloud/a2a', status: 401, body: 'JSON-RPC error -32001 Unauthorized, data.hint \"Authorization: Bearer <token>\"'}\n  - {url: 'GET https://humanbrowser.cloud/api/usage', status: 401, body: '{\"error\":\"Unauthorized. Pass Authorization: Bearer <DEPLOY_SECRET>\"}', note: 'the live route asks for a deployment secret, not a customer token'}\n  rules: ['never put the token in a URL query string (agent card)', 'the MCP endpoint refuses non-Bearer auth', 'tokens are hashed at rest (Privacy 10)', 'report a suspected compromise by email (Terms 3)']\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n  -\
  \ https://humanbrowser.cloud/docs/mcp\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: hb_session\n  description: Login session cookie for account endpoints.\n  used_by: [getAccount]\n  observed:\n  - {url: 'GET https://humanbrowser.cloud/api/account', status: 400, body: '{\"error\":\"bad-token\"}', note: 'without a cookie or token'}\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://agent.humanbrowser.cloud/oauth/token\n    scopes: 3\n    scope_list: [session:run, account:read, account:topup]\n  description: Least-privilege scoped access. Request only the scopes an agent needs.\n  used_by: [getAccount (account:read), topUp (account:topup), getUsage (account:read), runA2ATask (session:run)]\n  status: declared but not reachable\n  observed:\n  - {url: 'https://agent.humanbrowser.cloud/oauth/token', method: GET, status: 404}\n  - {url: 'https://agent.humanbrowser.cloud/oauth/token',\
  \ method: POST, status: 404, body: '{\"error\":\"not-found\",\"path\":\"/oauth/token\"}'}\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n- name: mcp-oauth (RFC 8414 / RFC 9728, not in the OpenAPI)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://agent.humanbrowser.cloud/authorize\n    tokenUrl: https://agent.humanbrowser.cloud/token\n    refreshUrl: https://agent.humanbrowser.cloud/token\n    registrationUrl: https://agent.humanbrowser.cloud/register\n    revocationUrl: https://agent.humanbrowser.cloud/revoke\n    pkce: S256 required (only method listed)\n    client_auth: [none, client_secret_post]\n    client_ids: 'CIMD URL (https://) or DCR id hbc_<32hex>'\n    scopes: [mcp:run, mcp:read]\n  resource: https://agent.humanbrowser.cloud/mcp\n  description: The OAuth 2.1 door an MCP client following RFC 9728 discovery would find; scopes and endpoints from the two well-known documents. No human-readable documentation exists for it.\n  status:\
  \ live but undocumented\n  observed:\n  - {url: 'GET /authorize', status: 400, body: 'unsupported_response_type — response_type must be code'}\n  - {url: 'GET /authorize?response_type=code&client_id=probe', status: 400, body: 'invalid_client — client_id must be CIMD URL (https://) or DCR id (hbc_<32hex>)'}\n  - {url: 'POST /token (empty form)', status: 400, body: 'unsupported_grant_type — grant_type must be authorization_code or refresh_token'}\n  - {url: 'GET /token', status: 404}\n  - {url: 'GET /register', status: 404, note: 'POST not attempted (would register a client)'}\n  - {url: 'https://humanbrowser.cloud/docs/oauth (service_documentation)', status: 404}\n  sources:\n  - well-known/humanbrowser-cloud-oauth-authorization-server.json\n  - well-known/humanbrowser-cloud-oauth-protected-resource.json\na2a_card_scheme:\n  http_bearer: {type: http, scheme: bearer, description: 'Skill token issued by humanbrowser.cloud. Required on every /a2a call.'}\n  security: [{http_bearer: []}]\n\
  environment_variables:\n  HB_TOKEN: canonical since 5.0.2 (stdio MCP server, CLI)\n  HUMANBROWSER_API_TOKEN: legacy alias, still accepted\n  HB_API_BASE / HUMANBROWSER_API_BASE: 'override the agent host (default https://agent.humanbrowser.cloud)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/authentication/humanbrowser-cloud-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Browser Automation
- Cloud Browser
- AI Agents
- A2A
- MCP
- Web Scraping
- Residential Proxies
- CAPTCHA Solving
- Human-in-the-Loop
- Computer Use
- Agent-Native
- United Kingdom
---
