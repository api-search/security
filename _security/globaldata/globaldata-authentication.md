---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Globaldata Authentication
name_suffix: Authentication
oauth_flows: []
overview: GlobalData declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: GlobalData
provider_slug: globaldata
scheme_count: 3
schemes:
- audience: Interactive MCP clients — claude.ai custom connectors, Microsoft Copilot Studio, browser-based agents. The user signs in through a browser window; no client secret is held by the agent.
  authorization_server: https://login.globaldata.com
  client_registration: Not dynamic. GlobalData requires the redirect URI to be registered with its Direct Data Solutions (DDS) team before first use.
  code_challenge_methods:
  - S256
  flow: authorization_code
  id: oauth2_authorization_code_pkce
  pkce: required
  source: https://mcp.globaldata.com/
  token_endpoint: https://login.globaldata.com/oauth/token
  type: oauth2
- audience: back-end agents, scripts, server-to-server automation
  expires_in: 3600
  flow: password
  id: oauth2_password
  label: Credentials grant
  note: Exchanges a GlobalData username and password directly for a bearer token. Documented by GlobalData for non-interactive agents.
  parameters:
  - grant_type
  - username
  - password
  - scope
  request_content_type: application/x-www-form-urlencoded
  scopes_requested:
  - openid
  - profile
  - email
  - offline_access
  source: https://mcp.globaldata.com/
  token_endpoint: https://login.globaldata.com/oauth/token
  token_type: Bearer
  type: oauth2
- declared_in: https://mcp.globaldata.com/.well-known/oauth-authorization-server
  flow: client_credentials
  id: oauth2_client_credentials
  note: Listed in grant_types_supported of the gateway's own RFC 8414 metadata. Not written up in the prose documentation, so recorded as declared-by-the-server rather than documented-for-callers.
  source: https://mcp.globaldata.com/.well-known/oauth-authorization-server
  type: oauth2
slug: globaldata-authentication
source_filename: globaldata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://mcp.globaldata.com/ (Section 04, Authentication) and the probed RFC 8414 document at\n  https://mcp.globaldata.com/.well-known/oauth-authorization-server\nsummary: >-\n  One authentication model across the whole published surface: OAuth 2.1 against GlobalData SSO.\n  There are no API keys, no basic auth, and no unauthenticated read path — every MCP endpoint\n  returns HTTP 401 with a WWW-Authenticate Bearer challenge until a token is presented. What a\n  token can actually see is decided by subscription entitlement, not by scope.\nderivation_note: >-\n  NOT derived from an OpenAPI securitySchemes block — no OpenAPI exists for this provider. Every\n  field below was read either from GlobalData's own developer documentation or from a discovery\n  document that was fetched and parsed.\nschemes:\n  - id: oauth2_authorization_code_pkce\n    type: oauth2\n    flow: authorization_code\n    pkce: required\n    code_challenge_methods:\
  \ [S256]\n    authorization_server: https://login.globaldata.com\n    token_endpoint: https://login.globaldata.com/oauth/token\n    audience: >-\n      Interactive MCP clients — claude.ai custom connectors, Microsoft Copilot Studio, browser-based\n      agents. The user signs in through a browser window; no client secret is held by the agent.\n    client_registration: >-\n      Not dynamic. GlobalData requires the redirect URI to be registered with its Direct Data\n      Solutions (DDS) team before first use.\n    source: https://mcp.globaldata.com/\n  - id: oauth2_password\n    type: oauth2\n    flow: password\n    label: Credentials grant\n    token_endpoint: https://login.globaldata.com/oauth/token\n    request_content_type: application/x-www-form-urlencoded\n    parameters: [grant_type, username, password, scope]\n    scopes_requested: [openid, profile, email, offline_access]\n    token_type: Bearer\n    expires_in: 3600\n    audience: back-end agents, scripts, server-to-server automation\n\
  \    note: >-\n      Exchanges a GlobalData username and password directly for a bearer token. Documented by\n      GlobalData for non-interactive agents.\n    source: https://mcp.globaldata.com/\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: client_credentials\n    declared_in: https://mcp.globaldata.com/.well-known/oauth-authorization-server\n    note: >-\n      Listed in grant_types_supported of the gateway's own RFC 8414 metadata. Not written up in the\n      prose documentation, so recorded as declared-by-the-server rather than documented-for-callers.\n    source: https://mcp.globaldata.com/.well-known/oauth-authorization-server\ntoken_presentation:\n  header: Authorization\n  format: 'Bearer <access_token>'\n  applies_to: every request to https://mcp.globaldata.com/{site}/mcp\nchallenge:\n  observed_status: 401\n  observed_body: '{\"error\":\"Unauthorized: token required\"}'\n  www_authenticate: >-\n    Bearer realm=\"GlobalData MCP\",\n    resource_metadata=\"https://mcp.globaldata.com/.well-known/oauth-protected-resource/mcp\"\
  \n  note: >-\n    RFC 9728-conformant challenge — the 401 names the protected-resource metadata document, which\n    is the behaviour an MCP client needs to discover the authorization server automatically.\n  checked: '2026-09-13'\nidentity_providers:\n  source: https://mcp.globaldata.com/ (Section 04)\n  options:\n    - GlobalData username and password\n    - Microsoft Entra ID\n    - Google Workspace\n    - Okta / enterprise SSO\nserver_metadata:\n  rfc_8414:\n    url: https://mcp.globaldata.com/.well-known/oauth-authorization-server\n    status: 200\n    issuer: https://mcp.globaldata.com\n    authorization_endpoint: https://mcp.globaldata.com/authorize\n    token_endpoint: https://mcp.globaldata.com/token\n    jwks_uri: https://mcp.globaldata.com/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token, client_credentials]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none,\
  \ client_secret_post, private_key_jwt]\n    token_endpoint_auth_signing_alg_values_supported: [RS256, PS256, ES256]\n    scopes_supported: [openid, profile, email, offline_access]\n    file: ../well-known/globaldata-mcp-oauth-authorization-server.json\n  rfc_9728:\n    url: https://mcp.globaldata.com/.well-known/oauth-protected-resource\n    status: 200\n    resource: https://mcp.globaldata.com\n    authorization_servers: [https://mcp.globaldata.com]\n    file: ../well-known/globaldata-mcp-oauth-protected-resource.json\n  discrepancy_note: >-\n    The gateway's RFC 8414 document names ITSELF as issuer with /authorize and /token on\n    mcp.globaldata.com, while the prose documentation tells callers to use login.globaldata.com.\n    Both are real: the gateway proxies or fronts GlobalData SSO. login.globaldata.com publishes no\n    RFC 8414 document of its own (its /.well-known/oauth-authorization-server 302s to an error\n    page), so the mcp.globaldata.com copy is the only machine-readable\
  \ server metadata GlobalData\n    publishes. A client following the RFC 9728 challenge lands on the working one.\nauthorization_model:\n  mechanism: subscription entitlement, evaluated server-side per credential\n  note: >-\n    Scopes are OIDC identity scopes only. Access to data is decided by what the caller's GlobalData\n    subscription includes: a vertical the subscription does not cover cannot be connected to, and a\n    domain it does not include will not reveal — discover_capabilities / reveal_advanced return a\n    not_entitled response rather than pretending to reveal it. Several domains carry their own\n    entitlement (contacts, market_data, fdi_projects, ict_contracts).\n  source: https://mcp.globaldata.com/ (Sections 03, 12)\nno_api_keys: >-\n  GlobalData publishes no API-key scheme for this surface. There is no key prefix, no key\n  management page, and no anonymous tier.\nchecked: '2026-09-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldata/refs/heads/main/authentication/globaldata-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Market Intelligence
- Business Intelligence
- Data
- Analytics
- MCP
- Agents
- Company Data
- Deals
- News
- Patents
- Research
- Financial-Services
- Energy
- Mining
---
