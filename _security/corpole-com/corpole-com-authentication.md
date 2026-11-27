---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CorPole Authentication
name_suffix: Authentication
oauth_flows: []
overview: CorPole declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CorPole
provider_slug: corpole-com
scheme_count: 3
schemes:
- applies_to:
  - https://corpole.com/api/mcp
  authorization_server_metadata: /.well-known/oauth-authorization-server (RFC 8414)
  client_registration: Dynamic (POST /api/oauth/register, RFC 7591) or Client ID Metadata Documents (an https client_id)
  flow: authorizationCode
  name: oauth2
  pkce: S256 (required); public clients
  protected_resource_metadata: /.well-known/oauth-protected-resource/api/mcp (RFC 9728)
  redirect_uris: https, or http on a loopback address (any port)
  revocation: POST /api/oauth/revoke (RFC 7009), or Disconnect on the solution's Agents page
  scopes:
  - read
  - propose
  token_lifetime: Access 1 hour, refresh 30 days with rotation; reusing a code or a refresh token revokes the connection
  type: oauth2
- applies_to:
  - https://corpole.com/api/mcp
  - https://corpole.com/api/context
  description: Personal token for one machine or tool, with an expiry; acts as its owner. Sent as Authorization Bearer. Tokens are shown once and stored only as a hash.
  name: personalToken
  scheme: bearer
  type: http
- applies_to:
  - https://corpole.com/api/context
  - CI change-request check
  description: Service token for CI (the change-request check and test results); acts as the person with the Integrations permission who created it. Stored as CORPOLE_TOKEN in CI.
  name: serviceToken
  scheme: bearer
  type: http
slug: corpole-com-authentication
source_filename: corpole-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://corpole.com/support/reference/oauth-details\n- https://corpole.com/support/connect-your-agent/tokens-and-identity\n- https://corpole.com/support/connect-your-agent/rest-and-claude-md-fallback\n- https://corpole.com/support/troubleshooting/401-invalid-token\ndocs: https://corpole.com/support/reference/oauth-details\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: [https://corpole.com/api/mcp]\n  flow: authorizationCode\n  pkce: S256 (required); public clients\n  authorization_server_metadata: /.well-known/oauth-authorization-server (RFC 8414)\n  protected_resource_metadata: /.well-known/oauth-protected-resource/api/mcp (RFC 9728)\n  client_registration: Dynamic (POST /api/oauth/register, RFC 7591) or Client ID Metadata Documents (an https client_id)\n  redirect_uris: https, or http on a loopback address (any port)\n  token_lifetime: Access 1 hour, refresh 30 days with rotation; reusing a code or a refresh\
  \ token revokes the connection\n  revocation: POST /api/oauth/revoke (RFC 7009), or Disconnect on the solution's Agents page\n  scopes: [read, propose]\n- name: personalToken\n  type: http\n  scheme: bearer\n  applies_to: [https://corpole.com/api/mcp, https://corpole.com/api/context]\n  description: Personal token for one machine or tool, with an expiry; acts as its owner. Sent as Authorization Bearer. Tokens are shown once and stored only as a hash.\n- name: serviceToken\n  type: http\n  scheme: bearer\n  applies_to: [https://corpole.com/api/context, CI change-request check]\n  description: Service token for CI (the change-request check and test results); acts as the person with the Integrations permission who created it. Stored as CORPOLE_TOKEN in CI.\nnotes:\n- A connection belongs to one solution and never has more permissions than the person it acts for.\n- Anonymous requests to the MCP endpoint get HTTP 401 (pre-flight probe observed 401 at https://corpole.com/api/mcp).\n"
source_yaml_url: https://artifacts.apis.io/corpole-com/authentication/corpole-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Agents
- Coding Agents
- MCP
- Requirements Management
- Governance
- Traceability
- Developer Tools
---
