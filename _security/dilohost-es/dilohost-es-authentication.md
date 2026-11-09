---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dilohost Es Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dilohost declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Dilohost
provider_slug: dilohost-es
scheme_count: 3
schemes:
- description: OAuth 2.1 authorization code with PKCE (S256 mandatory) and RFC 8707 resource indicator resource=https://mcp.dilohost.es/mcp. Public clients only (token_endpoint_auth_methods_supported none). Clients identify via Client ID Metadata Document (preferred; only trusted clients Claude Code, claude.ai/Claude Desktop and Codex accepted) or dynamic client registration (RFC 7591, max 20 registrations per hour and IP).
  discovery:
    authorization_server_metadata: https://dilohost.es/.well-known/oauth-authorization-server
    protected_resource_metadata: https://mcp.dilohost.es/.well-known/oauth-protected-resource
    www_authenticate: Bearer realm="mcp", resource_metadata="https://mcp.dilohost.es/.well-known/oauth-protected-resource/mcp", scope="mcp:use"
  errors:
    insufficient_scope: 403 insufficient_scope
    missing_token: 401 with WWW-Authenticate
    wrong_resource: invalid_target
  flows:
    authorizationCode:
      authorizationUrl: https://dilohost.es/oauth/authorize
      registrationUrl: https://dilohost.es/oauth/register
      scopes:
        mcp:use: Access to the Dilohost MCP server
      tokenUrl: https://dilohost.es/oauth/token
  id: oauth2
  tokens:
    access_token: 1 hour, JWT with RFC 9068 profile (typ at+jwt); audience includes the MCP URL
    refresh_token: 30 days, rotated on every use; reuse of a spent token revokes all access for that client and person
  type: oauth2
- description: Service tokens created by the account owner in the panel (Ajustes -> Tokens de servicio), prefix dhs_, valid 1 to 365 days, up to 20 active per account, shown once (only a hash is stored). Sent as Authorization Bearer dhs_... Acts as a team member, not as owner (no team, plan, payments or spend cap).
  docs: https://dilohost.es/docs/cuenta/tokens
  id: serviceToken
  prefix: dhs_
  scheme: bearer
  type: http
- description: Requests carrying an Origin header not on the allow-list receive 403 with JSON-RPC error -32600 "Origin no permitido." (DNS-rebinding protection).
  id: originValidation
  type: note
slug: dilohost-es-authentication
source_filename: dilohost-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dilohost.es/docs/referencia/servidor-mcp\ndocs: https://dilohost.es/docs/referencia/servidor-mcp\nname: Dilohost authentication\nnote: Dilohost publishes no OpenAPI; this profile is read from the MCP server reference and the service-token page. Values are as documented, not observed (no token or OAuth endpoint was called).\nschemes:\n- id: oauth2\n  type: oauth2\n  description: OAuth 2.1 authorization code with PKCE (S256 mandatory) and RFC 8707 resource indicator resource=https://mcp.dilohost.es/mcp. Public clients only (token_endpoint_auth_methods_supported none). Clients identify via Client ID Metadata Document (preferred; only trusted clients Claude Code, claude.ai/Claude Desktop and Codex accepted) or dynamic client registration (RFC 7591, max 20 registrations per hour and IP).\n  flows:\n    authorizationCode:\n      authorizationUrl: https://dilohost.es/oauth/authorize\n      tokenUrl: https://dilohost.es/oauth/token\n\
  \      registrationUrl: https://dilohost.es/oauth/register\n      scopes:\n        mcp:use: Access to the Dilohost MCP server\n  discovery:\n    protected_resource_metadata: https://mcp.dilohost.es/.well-known/oauth-protected-resource\n    authorization_server_metadata: https://dilohost.es/.well-known/oauth-authorization-server\n    www_authenticate: 'Bearer realm=\"mcp\", resource_metadata=\"https://mcp.dilohost.es/.well-known/oauth-protected-resource/mcp\", scope=\"mcp:use\"'\n  tokens:\n    access_token: 1 hour, JWT with RFC 9068 profile (typ at+jwt); audience includes the MCP URL\n    refresh_token: 30 days, rotated on every use; reuse of a spent token revokes all access for that client and person\n  errors:\n    missing_token: 401 with WWW-Authenticate\n    insufficient_scope: 403 insufficient_scope\n    wrong_resource: invalid_target\n- id: serviceToken\n  type: http\n  scheme: bearer\n  description: Service tokens created by the account owner in the panel (Ajustes -> Tokens de servicio),\
  \ prefix dhs_, valid 1 to 365 days, up to 20 active per account, shown once (only a hash is stored). Sent as Authorization Bearer dhs_... Acts as a team member, not as owner (no team, plan, payments or spend cap).\n  prefix: dhs_\n  docs: https://dilohost.es/docs/cuenta/tokens\n- id: originValidation\n  type: note\n  description: Requests carrying an Origin header not on the allow-list receive 403 with JSON-RPC error -32600 \"Origin no permitido.\" (DNS-rebinding protection).\n"
source_yaml_url: https://artifacts.apis.io/dilohost-es/authentication/dilohost-es-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Hosting
- Web Hosting
- MCP
- AI Agents
- Database
- Domains
- Email
- European Union
---
