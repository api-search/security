---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Stellary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stellary declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Stellary
provider_slug: stellary
scheme_count: 3
schemes:
- accepted_credentials:
  - identity: human user
    issued_by: POST /auth/login and the other /auth flows
    kind: user_jwt
    note: Response returns a temporary two-factor token instead of a session when 2FA is required.
  - expiry: optional ISO expiresAt at creation
    identity: human user
    issued_by: POST /api-tokens
    kind: personal_access_token
    prefix: sl_
    prefix_evidence: Docs example response returns tokenPrefix "sl_abcd12"; the secret is returned once at creation only.
    scoped: true
    valid_for:
    - REST
    - MCP
  - identity: workspace agent
    kind: agent_token
    used_for: queued missions, stellary_init, installed plugin tools
  - identity: anonymous transport context
    kind: mcp_token
    note: Transport gate only. Documented as insufficient for tools that require a user or agent identity, and only reachable when NODE_ENV is not production and MCP_TOKEN is unset.
  applies_to:
  - REST
  - MCP
  format: Bearer <jwt-or-personal-access-token>
  header: Authorization
  id: bearer
  in: header
  scheme: bearer
  type: http
- access_token_lifetime: 1 hour
  applies_to:
  - MCP
  dynamic_client_registration:
    endpoint: https://api.stellary.co/register
    standard: RFC 7591
    supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://api.stellary.co/authorize
      pkce: required (S256)
      refreshUrl: https://api.stellary.co/token
      scopes:
        offline_access: Issue a rotating refresh token
        pilotage:read: Read cockpit/pilotage state, dashboards and proposals
        pilotage:write: Create and act on pilotage actions and proposals
        projects:read: Read projects, boards, cards and delivery context
        projects:write: Create and modify projects, cards, comments and assignments
      tokenUrl: https://api.stellary.co/token
  id: oauth2
  profile: OAuth 2.1
  refresh: rotating refresh token when offline_access is granted
  revocation_endpoint: https://api.stellary.co/revoke
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
- applies_to:
  - REST
  id: session_cookie
  in: cookie
  note: Fallback used by the first-party web app. A CSRF token is returned by /auth/login and /auth/me. Not intended for third-party integrations.
  type: apiKey
slug: stellary-authentication
source_filename: stellary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://stellary.co/docs/api/ + https://stellary.co/docs/mcp/ + probed https://api.stellary.co/.well-known/oauth-authorization-server\ndocs: https://stellary.co/docs/api/\nnote: >-\n  Derived by hand from the provider's own reference pages and the live RFC 8414 metadata, not\n  from an OpenAPI securitySchemes block -- Stellary publishes no machine-readable contract\n  (Swagger UI is mounted at /api/docs in non-production builds only, per their API reference).\nsummary: >-\n  One Bearer scheme covers both surfaces. The backend guard tries the Authorization header first\n  and falls back to the web app's authenticated session cookie. For MCP clients, OAuth 2.1 with\n  PKCE and dynamic client registration is the recommended and discoverable path.\nschemes:\n- id: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <jwt-or-personal-access-token>'\n  applies_to: [REST, MCP]\n  accepted_credentials:\n\
  \  - kind: user_jwt\n    issued_by: POST /auth/login and the other /auth flows\n    identity: human user\n    note: Response returns a temporary two-factor token instead of a session when 2FA is required.\n  - kind: personal_access_token\n    issued_by: POST /api-tokens\n    identity: human user\n    prefix: sl_\n    prefix_evidence: 'Docs example response returns tokenPrefix \"sl_abcd12\"; the secret is returned once at creation only.'\n    scoped: true\n    expiry: optional ISO expiresAt at creation\n    valid_for: [REST, MCP]\n  - kind: agent_token\n    identity: workspace agent\n    used_for: queued missions, stellary_init, installed plugin tools\n  - kind: mcp_token\n    identity: anonymous transport context\n    note: >-\n      Transport gate only. Documented as insufficient for tools that require a user or agent\n      identity, and only reachable when NODE_ENV is not production and MCP_TOKEN is unset.\n- id: oauth2\n  type: oauth2\n  profile: OAuth 2.1\n  applies_to: [MCP]\n  flows:\n\
  \    authorizationCode:\n      authorizationUrl: https://api.stellary.co/authorize\n      tokenUrl: https://api.stellary.co/token\n      refreshUrl: https://api.stellary.co/token\n      pkce: required (S256)\n      scopes:\n        projects:read: Read projects, boards, cards and delivery context\n        projects:write: Create and modify projects, cards, comments and assignments\n        pilotage:read: Read cockpit/pilotage state, dashboards and proposals\n        pilotage:write: Create and act on pilotage actions and proposals\n        offline_access: Issue a rotating refresh token\n  dynamic_client_registration:\n    supported: true\n    endpoint: https://api.stellary.co/register\n    standard: RFC 7591\n  revocation_endpoint: https://api.stellary.co/revoke\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  access_token_lifetime: 1 hour\n  refresh: rotating refresh token when offline_access is granted\n- id: session_cookie\n  type: apiKey\n  in: cookie\n  applies_to:\
  \ [REST]\n  note: >-\n    Fallback used by the first-party web app. A CSRF token is returned by /auth/login and\n    /auth/me. Not intended for third-party integrations.\nidentity_model:\n  note: >-\n    An OAuth connection belongs to one workspace and may authorize the human, one or more active\n    workspace agents, or both. With a single identity actingAs is implicit; with several it is\n    required on every call, including stellary_init and mission tools.\n  resolver_tool: stellary_list_identities\n  rechecked_per_call: [credential scopes, project access, workspace permissions, agent status, agent tool policy, autonomy mode, mission snapshot]\nmfa:\n  supported: true\n  note: Two-factor authentication is supported on user accounts; /auth/login returns a temporary two-factor token when it is required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellary/refs/heads/main/authentication/stellary-authentication.yml
summary_line: 3 schemes
tags:
- project-management
- productivity
- AI-agents
- agent-orchestration
- MCP
- remote-mcp
- developer-tools
- SaaS
- collaboration
---
