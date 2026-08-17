---
api_key_in: []
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Tdaycom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tdaycom secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tdaycom
provider_slug: tdaycom
scheme_count: 2
schemes:
- authorization_endpoint: https://tday.com/api/mcp/oauth/authorize
  authorization_server: https://tday.com
  challenge: 'WWW-Authenticate: Bearer resource_metadata="https://tday.com/.well-known/oauth-protected-resource/api/mcp"'
  dynamic_client_registration: true
  flow: authorizationCode
  name: OAuth2
  pkce: S256
  protects:
  - https://tday.com/api/mcp
  public_client: true
  registration_endpoint: https://tday.com/api/mcp/oauth/register
  revocation_endpoint: https://tday.com/api/mcp/oauth/revoke
  scopes:
  - tday
  sources:
  - well-known/tdaycom-oauth-authorization-server.json
  - well-known/tdaycom-oauth-protected-resource.json
  token_endpoint: https://tday.com/api/mcp/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  used_by:
  - Claude custom connector / remote MCP clients
- format: Bearer <token>
  header: authorization
  issuance: Not self-serve from a dashboard key page. `npx -y @designtday/mcp install` opens tday.com in the browser on a loopback callback bound to 127.0.0.1 with a random `state` nonce; the user signs in and authorizes the machine, and the token is written to ~/.tday/config.json with 0600 permissions. TDAY_TOKEN in the environment overrides the file.
  name: BearerToken
  protects:
  - https://tday.com/api/*
  revocation: Revocable from tday integrations/settings, per https://tday.com/mcp.
  scheme: bearer
  sources:
  - '@designtday/mcp v0.0.1 dist/config.js'
  - '@designtday/mcp v0.0.1 dist/tools.js'
  token_prefix: none-published
  type: http
  used_by:
  - '@designtday/mcp local stdio server'
  - '@designtday/mcp one-shot CLI (`call`)'
slug: tdaycom-authentication
source_filename: tdaycom-authentication.yml
source_heading: Authentication Profile
source_url: https://tday.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://tday.com/.well-known/oauth-authorization-server\ndocs: https://tday.com/mcp\nsources:\n- https://tday.com/.well-known/oauth-authorization-server\n- https://tday.com/.well-known/oauth-protected-resource\n- https://tday.com/.well-known/oauth-protected-resource/api/mcp\n- https://tday.com/mcp\n- '@designtday/mcp v0.0.1 dist/config.js + dist/tools.js (npm)'\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  note: >-\n    tday has no published OpenAPI. This profile combines its live OAuth 2.1 discovery\n    metadata (RFC 8414 + RFC 9728) with the token handling documented and implemented in\n    its own first-party npm client. Two authentication paths exist and they terminate in\n    the same place: an OAuth 2.1 authorization-code + PKCE flow for the hosted MCP\n    endpoint, and a browser-linked bearer token written to local disk for the stdio MCP\n    server and\
  \ CLI. There is no API-key issuance surface at all — no key page, no key\n    prefix, no header alternative.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  public_client: true\n  token_endpoint_auth_methods_supported:\n  - none\n  authorization_server: https://tday.com\n  authorization_endpoint: https://tday.com/api/mcp/oauth/authorize\n  token_endpoint: https://tday.com/api/mcp/oauth/token\n  registration_endpoint: https://tday.com/api/mcp/oauth/register\n  revocation_endpoint: https://tday.com/api/mcp/oauth/revoke\n  scopes:\n  - tday\n  protects:\n  - https://tday.com/api/mcp\n  challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://tday.com/.well-known/oauth-protected-resource/api/mcp\"'\n  used_by:\n  - Claude custom connector / remote MCP clients\n  sources:\n  - well-known/tdaycom-oauth-authorization-server.json\n  - well-known/tdaycom-oauth-protected-resource.json\n- name: BearerToken\n  type:\
  \ http\n  scheme: bearer\n  header: authorization\n  format: 'Bearer <token>'\n  token_prefix: none-published\n  protects:\n  - https://tday.com/api/*\n  issuance: >-\n    Not self-serve from a dashboard key page. `npx -y @designtday/mcp install` opens\n    tday.com in the browser on a loopback callback bound to 127.0.0.1 with a random\n    `state` nonce; the user signs in and authorizes the machine, and the token is written\n    to ~/.tday/config.json with 0600 permissions. TDAY_TOKEN in the environment\n    overrides the file.\n  revocation: Revocable from tday integrations/settings, per https://tday.com/mcp.\n  used_by:\n  - '@designtday/mcp local stdio server'\n  - '@designtday/mcp one-shot CLI (`call`)'\n  sources:\n  - '@designtday/mcp v0.0.1 dist/config.js'\n  - '@designtday/mcp v0.0.1 dist/tools.js'\nunauthenticated_behavior:\n  endpoint: https://tday.com/api/mcp\n  status: 401\n  body: '{\"error\":\"Unauthorized\"}'\n  checked: '2026-08-13'\nmfa_sso:\n  sso_published: false\n\
  \  note: SSO appears on https://tday.com/pricing only as a feature of the unpriced Scale tier, not as a documented, available authentication option.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tdaycom/refs/heads/main/authentication/tdaycom-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Marketing
- Artificial Intelligence
- Content Generation
- Design
- Video
- Social Media
- Developer Tools
- MCP
- Agents
- Y Combinator
---
