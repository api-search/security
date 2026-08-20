---
api_key_in:
- header
- query
api_specs:
- filename: rybbit-analytics-api-openapi.yml
  format: yaml
  label: Rybbit Analytics API
  slug: rybbit-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-analytics-api-openapi.yml
- filename: rybbit-event-tracking-api-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-event-tracking-api-openapi.yml
- filename: rybbit-sessions-api-openapi.yml
  format: yaml
  label: Rybbit Sessions API
  slug: rybbit-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-sessions-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Rybbit authenticates every API and MCP request with one of three credentials: an organization API key, a personal API key, or an OAuth 2.1 access token issued by Rybbit''s own authorization server for the hosted MCP endpoint. The OpenAPI in this repo only expresses the bearer scheme; the rest of this profile was read from Rybbit''s published auth documentation and the RFC 8414 / RFC 9728 discovery documents saved under well-known/.'
kind: authentication
layout: security
method: searched
name: Rybbit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rybbit secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rybbit
provider_slug: rybbit
scheme_count: 3
schemes:
- description: 'User- or organization-scoped API key sent as `Authorization: Bearer <key>`. Organization keys (prefix `rb_org_`) belong to the organization, reach every site in it, and survive staff turnover; only organization admins/owners can create them (Settings > Organization > Organization API Keys). Personal keys act as the individual user with exactly their access across every organization they belong to (Settings > Account > Personal API Keys) and are the recommended credential for MCP clients. Either kind can be created with a `permissions` object restricting it to `resource:action` scopes; leave restrictions off for a full-access key. Keys are shown once at creation.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rybbit-openapi.yml
  - https://rybbit.com/docs/api/getting-started
  - https://rybbit.com/docs/account-settings
  type: http
- deprecated_for_production: true
  description: '`?api_key=<key>` is accepted on the Stats API for quick testing ONLY — Rybbit''s own docs warn it leaks the key into server logs and browser history. It is NOT accepted on the MCP endpoint.'
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - https://rybbit.com/docs/api/getting-started
  type: apiKey
- description: OAuth 2.1 authorization code + PKCE (S256) with RFC 7591 dynamic client registration, used by MCP clients that support the MCP authorization flow (Claude Code, Codex, Claude Desktop, opencode). Discovered from /.well-known/oauth-protected-resource on the API host. Tokens act with the granting user's role and share that user's rate-limit budget.
  detail: scopes/rybbit-scopes.yml
  flows:
  - authorizationUrl: https://app.rybbit.io/api/auth/mcp/authorize
    flow: authorizationCode
    scopes: 29
    tokenUrl: https://app.rybbit.io/api/auth/mcp/token
  name: RybbitMCP
  sources:
  - well-known/rybbit-oauth-authorization-server.json
  - well-known/rybbit-oauth-protected-resource.json
  - https://rybbit.com/docs/mcp
  type: oauth2
slug: rybbit-authentication
source_filename: rybbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/rybbit-openapi.yml\ndocs: https://rybbit.com/docs/api/getting-started\ndescription: >-\n  Rybbit authenticates every API and MCP request with one of three credentials:\n  an organization API key, a personal API key, or an OAuth 2.1 access token\n  issued by Rybbit's own authorization server for the hosted MCP endpoint. The\n  OpenAPI in this repo only expresses the bearer scheme; the rest of this\n  profile was read from Rybbit's published auth documentation and the RFC 8414\n  / RFC 9728 discovery documents saved under well-known/.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\n  scopes: 29\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      User- or organization-scoped API key sent as `Authorization: Bearer <key>`.\n      Organization keys (prefix `rb_org_`) belong to the organization, reach\
  \ every\n      site in it, and survive staff turnover; only organization admins/owners can\n      create them (Settings > Organization > Organization API Keys). Personal keys\n      act as the individual user with exactly their access across every\n      organization they belong to (Settings > Account > Personal API Keys) and are\n      the recommended credential for MCP clients. Either kind can be created with\n      a `permissions` object restricting it to `resource:action` scopes; leave\n      restrictions off for a full-access key. Keys are shown once at creation.\n    sources:\n      - openapi/rybbit-openapi.yml\n      - https://rybbit.com/docs/api/getting-started\n      - https://rybbit.com/docs/account-settings\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: >-\n      `?api_key=<key>` is accepted on the Stats API for quick testing ONLY —\n      Rybbit's own docs warn it leaks the key into server logs and browser\n      history. It\
  \ is NOT accepted on the MCP endpoint.\n    deprecated_for_production: true\n    sources:\n      - https://rybbit.com/docs/api/getting-started\n  - name: RybbitMCP\n    type: oauth2\n    description: >-\n      OAuth 2.1 authorization code + PKCE (S256) with RFC 7591 dynamic client\n      registration, used by MCP clients that support the MCP authorization flow\n      (Claude Code, Codex, Claude Desktop, opencode). Discovered from\n      /.well-known/oauth-protected-resource on the API host. Tokens act with the\n      granting user's role and share that user's rate-limit budget.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.rybbit.io/api/auth/mcp/authorize\n        tokenUrl: https://app.rybbit.io/api/auth/mcp/token\n        scopes: 29\n    detail: scopes/rybbit-scopes.yml\n    sources:\n      - well-known/rybbit-oauth-authorization-server.json\n      - well-known/rybbit-oauth-protected-resource.json\n      - https://rybbit.com/docs/mcp\ningestion:\n\
  \  endpoint: POST /api/track\n  auth: optional\n  note: >-\n    The public ingestion endpoint accepts unauthenticated writes from the\n    tracking script (the site is resolved from `site_id`). An API key is\n    optional but recommended for server-side tracking because it bypasses bot\n    detection and domain validation.\nauthorization:\n  model: role + scope\n  roles: [member, admin, owner]\n  note: >-\n    Scopes filter what a credential MAY attempt; the organization role still\n    decides what it MAY DO. Admin/owner-only operations refuse a member-role\n    credential with 403 regardless of scope.\nself_hosted:\n  note: >-\n    Self-hosted (AGPL-3.0) instances run the same auth stack on the operator's\n    own BASE_URL, including the MCP authorization server at\n    /api/auth/mcp/* and the well-known documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/authentication/rybbit-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open-Source
- Cookieless
---
