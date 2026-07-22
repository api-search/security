---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wato Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Wato secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Wato
provider_slug: wato
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://qualified-tree-19-staging.authkit.app/oauth2/introspection
  issuer: https://qualified-tree-19-staging.authkit.app
  jwks_uri: https://qualified-tree-19-staging.authkit.app/oauth2/jwks
  name: watoOAuth
  registration_endpoint: https://qualified-tree-19-staging.authkit.app/oauth2/register
  sources:
  - well-known/wato-oauth-authorization-server.json
  - well-known/wato-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: wato-authentication
source_filename: wato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mesh.watolabs.com/.well-known/oauth-authorization-server\ndocs: https://docs.watolabs.com/docs/connect-clients\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  bearer_methods:\n  - header\n  notes: >-\n    The Wato MCP gateway (https://mesh.watolabs.com/api/mcp) is an OAuth 2.0\n    protected resource (RFC 9728 metadata published at\n    /.well-known/oauth-protected-resource). Authorization is delegated to a\n    WorkOS AuthKit authorization server (RFC 8414 metadata published), with\n    PKCE (S256), dynamic client registration, refresh tokens, and the device\n    authorization grant. MCP clients (Claude Code, Codex, Cursor) trigger the\n    OAuth flow interactively on connect; login, SSO, and directory sync are\n    handled by WorkOS. Agents never receive raw connector credentials — the\n    gateway executes approved connector tools server-side.\nschemes:\n- name: watoOAuth\n\
  \  type: oauth2\n  issuer: https://qualified-tree-19-staging.authkit.app\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/authorize\n    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token\n    pkce_methods:\n    - S256\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/device_authorization\n    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  registration_endpoint: https://qualified-tree-19-staging.authkit.app/oauth2/register\n  introspection_endpoint: https://qualified-tree-19-staging.authkit.app/oauth2/introspection\n  jwks_uri: https://qualified-tree-19-staging.authkit.app/oauth2/jwks\n  sources:\n  - well-known/wato-oauth-authorization-server.json\n\
  \  - well-known/wato-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wato/refs/heads/main/authentication/wato-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Agent Governance
- Team Memory
- Connectors
- Agent Skills
- Automation
- Developer Tools
- Y Combinator
---
