---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sapiom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Sapiom secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Sapiom
provider_slug: sapiom
scheme_count: 3
schemes:
- description: 'All REST API endpoints authenticate with a Bearer token: `Authorization: Bearer YOUR_API_KEY`. Keys are minted in the Sapiom Dashboard (https://app.sapiom.ai/settings) and read from the SAPIOM_API_KEY environment variable by the SDKs. Attribution (agentName) is set on the client to route spend to per-agent transaction history and spending rules.'
  name: BearerApiKey
  scheme: bearer
  sources:
  - https://docs.sapiom.ai/api-reference/introduction
  type: http
- description: The remote MCP resource (https://api.sapiom.ai/v1/mcp) is guarded by OAuth 2.0 with Protected Resource Metadata (RFC 9728) and Authorization Server Metadata (RFC 8414). Supports PKCE (S256), Dynamic Client Registration (RFC 7591), and the OAuth 2.0 Device Authorization Grant. Token endpoint auth method is "none" (public clients).
  flows:
  - authorizationUrl: https://api.sapiom.ai/v1/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.sapiom.ai/v1/oauth/token
  - flow: deviceCode
    tokenUrl: https://api.sapiom.ai/v1/oauth/token
  - flow: refreshToken
    tokenUrl: https://api.sapiom.ai/v1/oauth/token
  issuer: https://api.sapiom.ai
  name: OAuth2
  registration_endpoint: https://api.sapiom.ai/v1/oauth/register
  sources:
  - well-known/sapiom-oauth-authorization-server.json
  - well-known/sapiom-oauth-protected-resource.json
  type: oauth2
- description: The local authoring MCP (@sapiom/mcp) uses sapiom_authenticate, a browser-based approval flow that caches the credential at ~/.sapiom/credentials.json for subsequent tool calls.
  name: DeveloperBrowserLogin
  sources:
  - https://docs.sapiom.ai/agents/reference
  type: oauth2
slug: sapiom-authentication
source_filename: sapiom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sapiom.ai/api-reference/introduction.md + https://docs.sapiom.ai/integration/sdk.md + well-known/sapiom-oauth-authorization-server.json\ndocs: https://docs.sapiom.ai/api-reference/introduction\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    All REST API endpoints authenticate with a Bearer token: `Authorization: Bearer YOUR_API_KEY`.\n    Keys are minted in the Sapiom Dashboard (https://app.sapiom.ai/settings) and read from the\n    SAPIOM_API_KEY environment variable by the SDKs. Attribution (agentName) is set on the client\n    to route spend to per-agent transaction history and spending rules.\n  sources: [https://docs.sapiom.ai/api-reference/introduction]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The remote MCP\
  \ resource (https://api.sapiom.ai/v1/mcp) is guarded by OAuth 2.0 with\n    Protected Resource Metadata (RFC 9728) and Authorization Server Metadata (RFC 8414).\n    Supports PKCE (S256), Dynamic Client Registration (RFC 7591), and the OAuth 2.0 Device\n    Authorization Grant. Token endpoint auth method is \"none\" (public clients).\n  issuer: https://api.sapiom.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.sapiom.ai/v1/oauth/authorize\n    tokenUrl: https://api.sapiom.ai/v1/oauth/token\n    pkce: S256\n  - flow: deviceCode\n    tokenUrl: https://api.sapiom.ai/v1/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://api.sapiom.ai/v1/oauth/token\n  registration_endpoint: https://api.sapiom.ai/v1/oauth/register\n  sources: [well-known/sapiom-oauth-authorization-server.json, well-known/sapiom-oauth-protected-resource.json]\n- name: DeveloperBrowserLogin\n  type: oauth2\n  description: >-\n    The local authoring MCP (@sapiom/mcp) uses sapiom_authenticate,\
  \ a browser-based approval\n    flow that caches the credential at ~/.sapiom/credentials.json for subsequent tool calls.\n  sources: [https://docs.sapiom.ai/agents/reference]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapiom/refs/heads/main/authentication/sapiom-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Ai
- AI Agents
- Agent Infrastructure
- Model Context Protocol
- API Gateway
- Payments
- Agentic Commerce
- Developer Tools
- SDK
---
