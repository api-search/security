---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Chronicle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Chronicle secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Chronicle
provider_slug: chronicle
scheme_count: 3
schemes:
- format: Bearer <API_KEY>
  in: header
  key_prefix: chr_
  name: apiKeyAuthorization
  notes: Workspace-scoped API key for the REST API at /api/v1. Created in Chronicle web app Settings -> API by a workspace admin; shown once. Keys are revoked (not hard-deleted) to preserve audit visibility. Requests are rate limited per key.
  parameter: Authorization
  scope: workspace
  type: apiKey
- format: <API_KEY>
  in: header
  name: apiKeyHeader
  notes: Alternative header form of the same workspace-scoped API key. Use one method consistently.
  parameter: x-api-key
  scope: workspace
  type: apiKey
- applies_to: MCP server (https://mcp.chroniclehq.com)
  authorization_server: https://login.chroniclehq.com
  flows:
  - authorizationUrl: https://login.chroniclehq.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://login.chroniclehq.com/oauth2/token
  - deviceAuthorizationUrl: https://login.chroniclehq.com/oauth2/device_authorization
    flow: deviceCode
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  name: mcpOAuth
  notes: The MCP path uses OAuth 2.0 against login.chroniclehq.com and carries a JWT bearer token. JWT-auth errors surface as JWT_INVALID / JWT_EXPIRED / JWT_WRONG_AUDIENCE / JWT_SIGNATURE_INVALID. MCP requests require workspace_id in body or query (else WORKSPACE_ID_REQUIRED).
  token_type: JWT
  type: oauth2
slug: chronicle-authentication
source_filename: chronicle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chroniclehq.com/authentication\ndocs: https://docs.chroniclehq.com/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_headers: [Authorization, x-api-key]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\nschemes:\n- name: apiKeyAuthorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <API_KEY>'\n  scope: workspace\n  key_prefix: chr_\n  notes: >-\n    Workspace-scoped API key for the REST API at /api/v1. Created in Chronicle web app\n    Settings -> API by a workspace admin; shown once. Keys are revoked (not hard-deleted)\n    to preserve audit visibility. Requests are rate limited per key.\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  format: '<API_KEY>'\n  scope: workspace\n  notes: Alternative header form of the same workspace-scoped API key. Use one method consistently.\n- name: mcpOAuth\n  type:\
  \ oauth2\n  applies_to: MCP server (https://mcp.chroniclehq.com)\n  authorization_server: https://login.chroniclehq.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.chroniclehq.com/oauth2/authorize\n    tokenUrl: https://login.chroniclehq.com/oauth2/token\n    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.chroniclehq.com/oauth2/device_authorization\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_type: JWT\n  notes: >-\n    The MCP path uses OAuth 2.0 against login.chroniclehq.com and carries a JWT bearer\n    token. JWT-auth errors surface as JWT_INVALID / JWT_EXPIRED / JWT_WRONG_AUDIENCE /\n    JWT_SIGNATURE_INVALID. MCP requests require workspace_id in body or query\n    (else WORKSPACE_ID_REQUIRED).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronicle/refs/heads/main/authentication/chronicle-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Cloud Saas
- Presentations
- Artificial Intelligence
- Productivity
- Content Generation
- Agents
- MCP
- Developer API
---
