---
api_key_in:
- header
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Armature Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Armature secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Armature
provider_slug: armature
scheme_count: 3
schemes:
- description: OAuth 2.0 authorization-code + PKCE for the hosted MCP server (mcp.armature.tech/mcp). Recommended read-access method; the client is challenged on first contact and completes authorization in the browser. Dynamic client registration (RFC 7591) is supported.
  flows:
  - authorizationUrl: https://app.armature.tech/api/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://app.armature.tech
    registrationUrl: https://app.armature.tech/api/mcp/oauth/register
    revocationUrl: https://app.armature.tech/api/mcp/oauth/revoke
    scopes:
      mcp: Read-only access to workspace agent-session analytics
    tokenUrl: https://app.armature.tech/api/mcp/oauth/token
  name: mcpOAuth
  sources:
  - .well-known/oauth-authorization-server
  - docs.armature.tech/armature-mcp/connect
  type: oauth2
- description: Workspace API key sent as a bearer token in the Authorization header to the MCP server. Created in Settings -> API keys. Governs read access; revocable from the dashboard.
  in: header
  name: workspaceApiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - docs.armature.tech/armature-mcp/connect
  type: http
- description: Write-only ingest key used by the TypeScript/Python/Go MCP-analytics SDKs to stream telemetry to Armature. Provided to the SDK via the ANALYTICS_INGEST_API_KEY environment variable; scoped per MCP server, minted once ("shown once — copy it"), rotatable/revocable per server. If the key is missing the SDK quietly no-ops.
  env_var: ANALYTICS_INGEST_API_KEY
  in: header
  name: ingestApiKey
  scope: write-only
  sources:
  - docs.armature.tech/quickstart
  - docs.armature.tech/sdks/python
  type: apiKey
slug: armature-authentication
source_filename: armature-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  docs.armature.tech (quickstart, sdks/*, armature-mcp/connect, security/privacy)\n  and live /.well-known/oauth-authorization-server + oauth-protected-resource.\n  Armature's published OpenAPI at docs.armature.tech/.armature/openapi.json was\n  retired to an empty stub, so this profile is documented, not spec-derived.\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code + PKCE for the hosted MCP server\n    (mcp.armature.tech/mcp). Recommended read-access method; the client is\n    challenged on first contact and completes authorization in the browser.\n    Dynamic client registration (RFC 7591) is supported.\n  flows:\n  - flow: authorizationCode\n    issuer: https://app.armature.tech\n    authorizationUrl: https://app.armature.tech/api/mcp/oauth/authorize\n    tokenUrl: https://app.armature.tech/api/mcp/oauth/token\n\
  \    registrationUrl: https://app.armature.tech/api/mcp/oauth/register\n    revocationUrl: https://app.armature.tech/api/mcp/oauth/revoke\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    scopes:\n      mcp: Read-only access to workspace agent-session analytics\n  sources: [.well-known/oauth-authorization-server, docs.armature.tech/armature-mcp/connect]\n- name: workspaceApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Workspace API key sent as a bearer token in the Authorization header to the\n    MCP server. Created in Settings -> API keys. Governs read access; revocable\n    from the dashboard.\n  in: header\n  parameter: Authorization\n  sources: [docs.armature.tech/armature-mcp/connect]\n- name: ingestApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Write-only ingest key used by the TypeScript/Python/Go MCP-analytics SDKs to\n    stream telemetry to Armature. Provided to the SDK via the\n    ANALYTICS_INGEST_API_KEY\
  \ environment variable; scoped per MCP server, minted\n    once (\"shown once — copy it\"), rotatable/revocable per server. If the key is\n    missing the SDK quietly no-ops.\n  env_var: ANALYTICS_INGEST_API_KEY\n  scope: write-only\n  sources: [docs.armature.tech/quickstart, docs.armature.tech/sdks/python]\ndocs: https://docs.armature.tech/armature-mcp/connect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armature/refs/heads/main/authentication/armature-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Agent Experience
- Model Context Protocol
- MCP
- Analytics
- Observability
- AI Agents
- Product Analytics
- Developer Tools
---
