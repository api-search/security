---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Improvado Authentication
name_suffix: Authentication
oauth_flows: []
overview: Improvado secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Improvado
provider_slug: improvado
scheme_count: 3
schemes:
- description: RFC 7617 HTTP Basic. Credentials (username:password, base64) are provisioned by Improvado for Embedded API access; the customer changes the password on first use. Required for workspace management and for calling POST /api/v3/token to mint a workspace-scoped Bearer token. Invalid credentials return 401 Unauthorized.
  name: basicAuth
  scheme: basic
  type: http
  used_for:
  - workspace management
  - token acquisition
- bearerFormat: opaque
  description: 'Workspace-scoped access token obtained from POST /api/v3/token. Sent as Authorization: Bearer <token>. Required for workspace-specific resources (connections, accounts, extracts, destinations, data tables, loads, recipes, roles, webhooks). Token TTL is 30 minutes, renewed on each authorized use; an invalid or expired token returns 401 Unauthorized.'
  name: bearerToken
  scheme: bearer
  type: http
  used_for:
  - workspace-scoped resources
- description: Cookie-based session used by embedded-UI (iframe) flows, combined with an X-IM-WORKSPACE-ID request header to scope the session to a workspace.
  in: cookie
  name: cookieSession
  parameterName: dts_session_id
  type: apiKey
  used_for:
  - embedded iframe UI
slug: improvado-authentication
source_filename: improvado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.improvado.io/auth\ndocs: https://developers.improvado.io/auth\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Two-stage model. HTTP Basic (RFC 7617) is used for workspace-management\n    operations and to obtain a workspace-scoped access token; the resulting Bearer\n    token is used for all workspace-scoped resources. A cookie/session variant\n    (dts_session_id) with an X-IM-WORKSPACE-ID header scopes embedded-UI sessions.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    RFC 7617 HTTP Basic. Credentials (username:password, base64) are provisioned by\n    Improvado for Embedded API access; the customer changes the password on first use.\n    Required for workspace management and for calling POST /api/v3/token to mint a\n    workspace-scoped Bearer token. Invalid credentials return 401 Unauthorized.\n\
  \  used_for: [workspace management, token acquisition]\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: >-\n    Workspace-scoped access token obtained from POST /api/v3/token. Sent as\n    Authorization: Bearer <token>. Required for workspace-specific resources\n    (connections, accounts, extracts, destinations, data tables, loads, recipes,\n    roles, webhooks). Token TTL is 30 minutes, renewed on each authorized use;\n    an invalid or expired token returns 401 Unauthorized.\n  used_for: [workspace-scoped resources]\n- name: cookieSession\n  type: apiKey\n  in: cookie\n  parameterName: dts_session_id\n  description: >-\n    Cookie-based session used by embedded-UI (iframe) flows, combined with an\n    X-IM-WORKSPACE-ID request header to scope the session to a workspace.\n  used_for: [embedded iframe UI]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improvado/refs/heads/main/authentication/improvado-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Analytics
- Data Pipeline
- ETL
- Advertising Data
- Business Intelligence
- Data Integration
- AI Agents
---
