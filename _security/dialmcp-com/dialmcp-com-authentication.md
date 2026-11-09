---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dialmcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DialMCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DialMCP
provider_slug: dialmcp-com
scheme_count: 1
schemes:
- access_token_lifetime: 1 hour (expires_in 3600)
  authorization_code_lifetime: 10 minutes, single-use
  authorization_endpoint: https://mcp.dialmcp.com/authorize
  authorization_server_metadata: https://mcp.dialmcp.com/.well-known/oauth-authorization-server
  bearer_methods:
  - header
  client_id_metadata_documents: false
  dynamic_client_registration: RFC 7591
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2
  issuer: https://mcp.dialmcp.com
  notes:
  - Tokens are never accepted in the query string.
  - Static bearer tokens are not accepted; only tokens issued through this flow.
  - Unauthenticated requests get HTTP 401 with WWW-Authenticate Bearer error="invalid_token" and resource_metadata.
  - The browser sign-in flow must finish within 10 minutes; five wrong SMS codes lock the flow.
  openid_connect: false
  pkce:
  - plain
  - S256
  protected_resource_metadata: https://mcp.dialmcp.com/.well-known/oauth-protected-resource/mcp
  refresh_token: rotating; the previous token keeps working until the next refresh
  registration_endpoint: https://mcp.dialmcp.com/register
  revocation: Not documented; "This does not revoke the grant on DialMCP's side" when a client is removed.
  scopes: none
  token_endpoint: https://mcp.dialmcp.com/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  token_format: opaque (not JWT)
  type: oauth2
slug: dialmcp-com-authentication
source_filename: dialmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dialmcp.com/docs/oauth\ndocs: https://dialmcp.com/docs/oauth\nname: DialMCP authentication\nsummary: OAuth 2.1 (authorization code + PKCE, refresh token) for the hosted remote MCP endpoint https://mcp.dialmcp.com/mcp; no API keys; sign-in verifies a US/Canadian mobile number by SMS, which becomes the caller ID.\nschemes:\n- id: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: [plain, S256]\n  issuer: https://mcp.dialmcp.com\n  authorization_endpoint: https://mcp.dialmcp.com/authorize\n  token_endpoint: https://mcp.dialmcp.com/token\n  registration_endpoint: https://mcp.dialmcp.com/register\n  dynamic_client_registration: RFC 7591\n  client_id_metadata_documents: false\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  protected_resource_metadata: https://mcp.dialmcp.com/.well-known/oauth-protected-resource/mcp\n  authorization_server_metadata:\
  \ https://mcp.dialmcp.com/.well-known/oauth-authorization-server\n  openid_connect: false\n  bearer_methods: [header]\n  scopes: none\n  token_format: opaque (not JWT)\n  access_token_lifetime: 1 hour (expires_in 3600)\n  refresh_token: rotating; the previous token keeps working until the next refresh\n  authorization_code_lifetime: 10 minutes, single-use\n  revocation: Not documented; \"This does not revoke the grant on DialMCP's side\" when a client is removed.\n  notes:\n  - Tokens are never accepted in the query string.\n  - Static bearer tokens are not accepted; only tokens issued through this flow.\n  - Unauthenticated requests get HTTP 401 with WWW-Authenticate Bearer error=\"invalid_token\" and resource_metadata.\n  - The browser sign-in flow must finish within 10 minutes; five wrong SMS codes lock the flow.\n"
source_yaml_url: https://artifacts.apis.io/dialmcp-com/authentication/dialmcp-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MCP
- AI Agents
- Phone Calls
- Voice AI
- Telephony
---
