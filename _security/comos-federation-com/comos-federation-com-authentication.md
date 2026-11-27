---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comos-federation-com-openapi.yml
  format: yaml
  label: ComOS Federation Gateway
  slug: comos-federation-gateway
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-federation-com/openapi/comos-federation-com-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ComOS Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComOS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ComOS
provider_slug: comos-federation-com
scheme_count: 1
schemes:
- authorization_url: https://mcp.comos-federation.com/oauth/authorize
  bearer_methods:
  - header
  dynamic_client_registration: https://mcp.comos-federation.com/oauth/register
  flows:
  - authorization_code
  - refresh_token
  - client_credentials
  jwks_uri: https://mcp.comos-federation.com/oauth/jwks
  metadata:
  - https://comos-federation.com/.well-known/oauth-authorization-server
  - https://comos-federation.com/.well-known/oauth-protected-resource
  name: oauth2
  note: Server card lists authorizationUrl/tokenUrl on comos-federation.com; the authorization-server metadata (issuer https://mcp.comos-federation.com) names the mcp. host. Endpoints recorded from metadata, not called.
  pkce: S256
  revocation_url: https://mcp.comos-federation.com/oauth/revoke
  scopes_ref: scopes/comos-federation-com-scopes.yml
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  token_url: https://mcp.comos-federation.com/oauth/token
  type: oauth2
slug: comos-federation-com-authentication
source_filename: comos-federation-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comos-federation.com/.well-known/mcp/server-card.json\ndocs: https://comos-federation.com/security\nnote: 'The OpenAPI (openapi.json) declares no securitySchemes or security requirements. Auth comes from the server card, the RFC 8414 / RFC 9728 metadata documents and the Security page, which says: \"The\n  agent surface authenticates with OAuth 2.1 + PKCE per the MCP spec; enterprise SSO via OIDC (Okta, Azure AD, any provider).\" llms.txt: \"Discovery, shopping, and read-only introspection need no token;\n  privileged writes use OAuth 2.1 + PKCE with per-tool scopes, and tokenless writes deny.\"'\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  pkce: S256\n  authorization_url: https://mcp.comos-federation.com/oauth/authorize\n  token_url: https://mcp.comos-federation.com/oauth/token\n  revocation_url: https://mcp.comos-federation.com/oauth/revoke\n\
  \  jwks_uri: https://mcp.comos-federation.com/oauth/jwks\n  dynamic_client_registration: https://mcp.comos-federation.com/oauth/register\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  bearer_methods:\n  - header\n  scopes_ref: scopes/comos-federation-com-scopes.yml\n  metadata:\n  - https://comos-federation.com/.well-known/oauth-authorization-server\n  - https://comos-federation.com/.well-known/oauth-protected-resource\n  note: Server card lists authorizationUrl/tokenUrl on comos-federation.com; the authorization-server metadata (issuer https://mcp.comos-federation.com) names the mcp. host. Endpoints recorded from metadata,\n    not called.\nanonymous_access: Discovery, shopping and read-only introspection need no token (llms.txt).\n"
source_yaml_url: https://artifacts.apis.io/comos-federation-com/authentication/comos-federation-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Commerce
- AI Agents
- MCP
- Federation
- Payments
- Self-Hosted
- Operating System
---
