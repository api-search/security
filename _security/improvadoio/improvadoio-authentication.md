---
api_key_in:
- cookie
- header
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Improvadoio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Improvado.io secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Improvado.io
provider_slug: improvadoio
scheme_count: 4
schemes:
- applies_to:
  - POST /api/v3/token
  - workspaces management
  name: basicAuth
  rfc: RFC 7617
  scheme: basic
  type: http
  usage: Workspace management and obtaining a workspace token. Credentials are provided by Improvado for Embedded API access. Invalid credentials return 401 Unauthorized.
- name: bearerToken
  scheme: bearer
  token_ttl_seconds: 1800
  type: http
  usage: Workspace-scoped resources (connections, accounts, extractions, etc.). Token is obtained from POST /api/v3/token. Token expiration is 30 minutes, renewed on each authorized request.
- companion_header: X-IM-WORKSPACE-ID
  in: cookie
  name: dts_session_id
  type: apiKey
  usage: Alternative for browser-based integrations. Requires the dts_session_id cookie plus the X-IM-WORKSPACE-ID header.
- applies_to:
  - MCP server
  name: oauth2
  type: oauth2
  usage: OAuth 2.0 is used to authenticate the Improvado MCP server against a customer's existing Improvado credentials.
slug: improvadoio-authentication
source_filename: improvadoio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.improvado.io/auth.md\ndocs: https://developers.improvado.io/auth\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [cookie, header]\n  notes: >-\n    The Improvado Embedded API v3 uses HTTP Basic for workspace-agnostic\n    operations, HTTP Bearer tokens for workspace-scoped operations, and a\n    cookie-based alternative for browser integrations. The Improvado MCP\n    server authenticates with OAuth 2.0.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    rfc: RFC 7617\n    usage: >-\n      Workspace management and obtaining a workspace token. Credentials are\n      provided by Improvado for Embedded API access. Invalid credentials\n      return 401 Unauthorized.\n    applies_to: [POST /api/v3/token, workspaces management]\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    usage: >-\n      Workspace-scoped resources (connections, accounts, extractions, etc.).\n  \
  \    Token is obtained from POST /api/v3/token. Token expiration is 30 minutes,\n      renewed on each authorized request.\n    token_ttl_seconds: 1800\n  - name: cookieAuth\n    type: apiKey\n    in: cookie\n    name: dts_session_id\n    usage: >-\n      Alternative for browser-based integrations. Requires the dts_session_id\n      cookie plus the X-IM-WORKSPACE-ID header.\n    companion_header: X-IM-WORKSPACE-ID\n  - name: oauth2\n    type: oauth2\n    usage: >-\n      OAuth 2.0 is used to authenticate the Improvado MCP server against a\n      customer's existing Improvado credentials.\n    applies_to: [MCP server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improvadoio/refs/heads/main/authentication/improvadoio-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Company
- Marketing
- Analytics
- Data Integration
- ETL
- Marketing Intelligence
- Data Pipeline
- MCP
- Webhooks
---
