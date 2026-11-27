---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ComplyLayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComplyLayer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ComplyLayer
provider_slug: complylayer-com
scheme_count: 2
schemes:
- authorization_url: https://app.complylayer.com/oauth/authorize
  dynamic_client_registration: true
  evidence: Sign-in uses OAuth 2.1 with PKCE. Access tokens last one hour and refresh tokens rotate, with reuse detection.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2
  note: Endpoint URLs are read from the authorization-server metadata document; none of them were called.
  pkce: S256
  registration_url: https://app.complylayer.com/api/oauth/register/
  revocation_url: https://app.complylayer.com/api/oauth/revoke/
  scopes:
  - mcp
  token_endpoint_auth_methods:
  - none
  token_lifetime: Access tokens last one hour and refresh tokens rotate, with reuse detection.
  token_url: https://app.complylayer.com/api/oauth/token/
  type: oauth2
- bearer_methods:
  - header
  evidence: Claude and Claude Code connect by signing in to ComplyLayer; other clients can use a personal token.
  name: personal-token
  note: The docs do not say how a personal token is issued or its format beyond being a token; the protected-resource metadata declares bearer_methods_supported [header].
  scheme: bearer
  type: http
slug: complylayer-com-authentication
source_filename: complylayer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://complylayer.com/features/mcp-server\n- https://complylayer.com/llms-full.txt\n- https://app.complylayer.com/.well-known/oauth-protected-resource\n- https://app.complylayer.com/.well-known/oauth-authorization-server\ndocs: https://complylayer.com/features/mcp-server\nsummary: The only published programmatic surface is the remote MCP server at https://app.complylayer.com/api/mcp/ (Streamable HTTP). Clients authenticate with OAuth 2.1 authorization code + PKCE (S256) or with a personal token sent as a bearer header. No OpenAPI is published, so this profile comes from the docs and the live OAuth discovery documents (both fetched with GET, HTTP 200).\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_url: https://app.complylayer.com/oauth/authorize\n  token_url: https://app.complylayer.com/api/oauth/token/\n  registration_url: https://app.complylayer.com/api/oauth/register/\n\
  \  revocation_url: https://app.complylayer.com/api/oauth/revoke/\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  scopes: [mcp]\n  dynamic_client_registration: true\n  token_lifetime: \"Access tokens last one hour and refresh tokens rotate, with reuse detection.\"\n  evidence: \"Sign-in uses OAuth 2.1 with PKCE. Access tokens last one hour and refresh tokens rotate, with reuse detection.\"\n  note: Endpoint URLs are read from the authorization-server metadata document; none of them were called.\n- name: personal-token\n  type: http\n  scheme: bearer\n  bearer_methods: [header]\n  evidence: \"Claude and Claude Code connect by signing in to ComplyLayer; other clients can use a personal token.\"\n  note: The docs do not say how a personal token is issued or its format beyond being a token; the protected-resource metadata declares bearer_methods_supported [header].\n"
source_yaml_url: https://artifacts.apis.io/complylayer-com/authentication/complylayer-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Governance
- Compliance
- EU AI Act
- Risk Management
- GDPR
- MCP
- Privacy
---
