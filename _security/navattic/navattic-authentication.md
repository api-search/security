---
api_key_in: []
api_specs:
- filename: navattic-website-openapi.json
  format: json
  label: Navattic API
  slug: navattic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/openapi/navattic-website-openapi.json
auth_types:
- oauth2
- http
description: 'Navattic''s authenticated developer surface is the hosted MCP server at https://app.navattic.com/api/mcp. It accepts two credentials against the same endpoint: an OAuth 2.1 authorization-code grant with PKCE and dynamic client registration, or a workspace Personal Access Token presented as an HTTP bearer token. Both are scope-limited and workspace-isolated. The published website OpenAPI declares no securitySchemes because its single operation (GET /api/health) is unauthenticated; there is no public REST product API to profile, so this artifact is searched from the docs and the RFC 8414 / RFC 9728 metadata rather than derived from a spec.

  '
kind: authentication
layout: security
method: searched
name: Navattic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Navattic secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Navattic
provider_slug: navattic
scheme_count: 2
schemes:
- applies_to: https://app.navattic.com/api/mcp
  clients_documented:
  - ChatGPT
  - Claude Desktop
  - Claude Code
  - Gemini Enterprise
  flows:
  - authorizationUrl: https://app.navattic.com/api/mcp/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://app.navattic.com
    registrationUrl: https://app.navattic.com/api/mcp/oauth/register
    response_types:
    - code
    revocationUrl: https://app.navattic.com/api/mcp/oauth/revoke
    scope_count: 11
    scopes_detail: scopes/navattic-scopes.yml
    tokenUrl: https://app.navattic.com/api/mcp/oauth/token
  name: NavatticMCPOAuth
  sources:
  - https://app.navattic.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://app.navattic.com/api/mcp
  clients_documented:
  - Cursor
  - VS Code
  - Windsurf
  - Codex
  - IBM Bob
  - Microsoft Copilot Studio
  creation:
    location: Settings > Workspace > Access Tokens
    max_active_per_user: 25
    shown_once: true
    who_can_create: Workspace Admins only
    who_can_view: Builders can view existing tokens but cannot create or revoke them
  credential: Personal Access Token
  expiration_days:
  - 7
  - 30
  - 60
  - 90
  - 180
  header: 'Authorization: Bearer <token>'
  name: NavatticPersonalAccessToken
  scheme: bearer
  scope_selection: Scopes are chosen per token at creation time
  sources:
  - https://docs.navattic.com/workspace/mcp-server
  type: http
slug: navattic-authentication
source_filename: navattic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.navattic.com/workspace/mcp-server\ndocs: https://docs.navattic.com/workspace/mcp-server\nalso_probed:\n  - https://app.navattic.com/.well-known/oauth-authorization-server\n  - https://app.navattic.com/.well-known/oauth-protected-resource\ndescription: >\n  Navattic's authenticated developer surface is the hosted MCP server at\n  https://app.navattic.com/api/mcp. It accepts two credentials against the same\n  endpoint: an OAuth 2.1 authorization-code grant with PKCE and dynamic client\n  registration, or a workspace Personal Access Token presented as an HTTP bearer\n  token. Both are scope-limited and workspace-isolated. The published website\n  OpenAPI declares no securitySchemes because its single operation\n  (GET /api/health) is unauthenticated; there is no public REST product API to\n  profile, so this artifact is searched from the docs and the RFC 8414 / RFC 9728\n  metadata rather than derived from a spec.\n\
  summary:\n  types: [oauth2, http]\n  api_key_in: []\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]\nschemes:\n  - name: NavatticMCPOAuth\n    type: oauth2\n    applies_to: https://app.navattic.com/api/mcp\n    sources: [https://app.navattic.com/.well-known/oauth-authorization-server]\n    flows:\n      - flow: authorizationCode\n        issuer: https://app.navattic.com\n        authorizationUrl: https://app.navattic.com/api/mcp/oauth/authorize\n        tokenUrl: https://app.navattic.com/api/mcp/oauth/token\n        registrationUrl: https://app.navattic.com/api/mcp/oauth/register\n        revocationUrl: https://app.navattic.com/api/mcp/oauth/revoke\n        grant_types: [authorization_code, refresh_token]\n        response_types: [code]\n        scope_count: 11\n        scopes_detail: scopes/navattic-scopes.yml\n    clients_documented: [ChatGPT, Claude Desktop, Claude Code, Gemini Enterprise]\n\
  \  - name: NavatticPersonalAccessToken\n    type: http\n    scheme: bearer\n    applies_to: https://app.navattic.com/api/mcp\n    sources: [https://docs.navattic.com/workspace/mcp-server]\n    credential: Personal Access Token\n    header: 'Authorization: Bearer <token>'\n    creation:\n      location: Settings > Workspace > Access Tokens\n      who_can_create: Workspace Admins only\n      who_can_view: Builders can view existing tokens but cannot create or revoke them\n      max_active_per_user: 25\n      shown_once: true\n    expiration_days: [7, 30, 60, 90, 180]\n    scope_selection: Scopes are chosen per token at creation time\n    clients_documented: [Cursor, VS Code, Windsurf, Codex, IBM Bob, Microsoft Copilot Studio]\nworkspace_identity:\n  sso:\n    supported: true\n    docs: https://docs.navattic.com/workspace/sso\n    note: Members can be required to authenticate through an identity provider such as Okta or Azure AD.\n  directory_sync:\n    supported: true\n    protocol: SCIM\n\
  \    docs: https://docs.navattic.com/workspace/directory-sync\n    note: Automatic user provisioning and deprovisioning.\n  roles: [Admin, Builder, Rep]\n  note: >\n    Workspace SSO/SCIM govern human members of the Navattic app, not API\n    credentials. No customer-facing OIDC discovery document is served on any\n    Navattic host (/.well-known/openid-configuration is 404 on www, app, and\n    api). The 200 at academy.navattic.com/.well-known/openid-configuration\n    belongs to Thinkific, not Navattic.\nwebhook_authentication:\n  outbound: true\n  docs: https://docs.navattic.com/integrations/webhook\n  note: >\n    Navattic signs nothing, but it will send an Authorization header on outbound\n    webhook deliveries when one is configured on the webhook —\n    \"Basic <credentials>\" or \"Bearer <token>\". There is no HMAC signature\n    header documented.\nx-evidence:\n  - {url: 'https://app.navattic.com/api/mcp', status: 401, note: 'anonymous POST returns \"Provide a valid access token\
  \ as a Bearer token in the Authorization header.\"'}\n  - {url: 'https://app.navattic.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://app.navattic.com/.well-known/oauth-protected-resource', status: 200}\n  - {url: 'https://app.navattic.com/.well-known/openid-configuration', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/authentication/navattic-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Interactive Demos
- Product Demo
- Sales Enablement
- Marketing
- No-Code
- Webhook
- CRM Integration
- Sales Automation
- MCP
- Agents
- Product Analytics
---
