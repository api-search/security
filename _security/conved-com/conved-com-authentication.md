---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: conved.com Authentication
name_suffix: Authentication
oauth_flows: []
overview: conved.com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: conved.com
provider_slug: conved-com
scheme_count: 2
schemes:
- applies_to:
  - REST API https://www.conved.com/api/v1
  - MCP https://www.conved.com/mcp
  - conved CLI
  description: 'Every request needs the header Authorization: Bearer <token>. Tokens are created in the account page, start with cvd_, can be shown/copied again and revoked at any time (programs using it stop working immediately). Accounts are free; sign-in is by e-mail with a 6-digit code.'
  name: bearerToken
  scheme: bearer
  token_prefix: cvd_
  type: http
- applies_to:
  - MCP https://www.conved.com/mcp
  description: MCP clients sign in with OAuth 2.1 automatically - /mcp answers 401 with a link to /.well-known/oauth-protected-resource/mcp, the client registers itself (dynamic client registration) and opens /oauth/authorize in the browser. PKCE S256, refresh tokens.
  metadata:
    authorization_server: https://www.conved.com/.well-known/oauth-authorization-server
    protected_resource: https://www.conved.com/.well-known/oauth-protected-resource/mcp
  name: mcpOAuth
  scopes_documented: false
  type: oauth2
slug: conved-com-authentication
source_filename: conved-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.conved.com/docs\ndocs: https://www.conved.com/docs\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  applies_to: [REST API https://www.conved.com/api/v1, MCP https://www.conved.com/mcp, conved CLI]\n  description: 'Every request needs the header Authorization: Bearer <token>. Tokens are created in the account page, start with cvd_, can be shown/copied again and revoked at any time (programs using it stop working immediately). Accounts are free; sign-in is by e-mail with a 6-digit code.'\n  token_prefix: cvd_\n- name: mcpOAuth\n  type: oauth2\n  applies_to: [MCP https://www.conved.com/mcp]\n  description: MCP clients sign in with OAuth 2.1 automatically - /mcp answers 401 with a link to /.well-known/oauth-protected-resource/mcp, the client registers itself (dynamic client registration) and opens /oauth/authorize in the browser. PKCE S256, refresh tokens.\n  metadata:\n    protected_resource: https://www.conved.com/.well-known/oauth-protected-resource/mcp\n\
  \    authorization_server: https://www.conved.com/.well-known/oauth-authorization-server\n  scopes_documented: false\n"
source_yaml_url: https://artifacts.apis.io/conved-com/authentication/conved-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- File Conversion
- Documents
- Image
- Media
- MCP
- CLI
- Developer Tools
---
