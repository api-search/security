---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Super Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: SUPER STUDIO declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: SUPER STUDIO
provider_slug: super-studio
scheme_count: 6
schemes:
- api: ecforce API v2
  description: Rails-style token authentication. The token belongs to an "API connection user" created in the ecforce admin under システム管理 > メンバー管理 (System Admin > Member Management); the access token and the API login password are shown once, immediately after issuance, and cannot be re-read afterwards. The API connection option is a paid contract add-on.
  evidence:
    file: src/lib/ecforce-sdk/shared/index.ts
    quote: 'Authorization: `Token token="${env.ECF_API_TOKEN}"`'
    repo: https://github.com/super-studio/ecforce_headless
  format: Token token="<access token>"
  id: ecforce_admin_token
  in: header
  name: Authorization
  type: apiKey
- api: ecforce API v2
  description: v2/customer authenticates as a shopper. The first-party headless sample signs in with POST /customers/sign_in and carries the resulting session for My Page-equivalent calls.
  evidence:
    file: src/lib/ecforce-sdk/customer/session/endpoints.ts
    repo: https://github.com/super-studio/ecforce_headless
  id: ecforce_customer_session
  scheme: session
  type: http
- api: ecforce AI Agent API
  description: An API key issued in the ecforce admin screens, supplied to the first-party server SDK as the AI_AGENT_API_KEY environment variable. The SDK sets the header internally and the published README does not name it, so the header name is recorded as unspecified rather than guessed.
  evidence:
    package: '@super_studio/ecforce-ai-agent-server'
    quote: '`AI_AGENT_API_KEY`: 必須。管理画面で発行した API キー'
    version: 1.5.0
  id: ai_agent_api_key
  in: header
  name: unspecified
  type: apiKey
- api: ecforce AI Agent API
  bearer_format: JWT
  description: Short-lived chat session tokens minted server-side by client.internalChat.createSession() and handed to the browser components. Shape is { token, expiresAt }. The SDK depends on jose and @panva/hkdf, so these are signed/derived tokens rather than opaque strings.
  id: agent_session_token
  scheme: bearer
  type: http
- api: ecforce AI Agent API
  description: MCP_TOKEN_SECRET signs and verifies MCP tokens when a tenant application exposes its own MCP tools alongside ecforce's. Required only when implementing MCP.
  id: mcp_token_secret
  in: header
  name: unspecified
  type: apiKey
- api: ecforce AI MCP
  authorization_url: https://agent.ec-force.com/mcp/oauth/authorize
  description: 'Public-client OAuth 2.1-shaped flow: no client secret, PKCE S256 mandatory, RFC 7591 dynamic client registration open to anonymous callers, refresh tokens supported. This is the pattern an MCP client is expected to complete on its own with no pre-registration.'
  evidence:
    status: 200
    url: https://agent.ec-force.com/.well-known/oauth-authorization-server
  flow: authorizationCode
  id: mcp_oauth
  pkce: S256
  registration_url: https://agent.ec-force.com/mcp/oauth/register
  revocation_url: https://agent.ec-force.com/mcp/oauth/revoke
  scopes:
  - mcp
  token_endpoint_auth_methods:
  - none
  token_url: https://agent.ec-force.com/mcp/oauth/token
  type: oauth2
slug: super-studio-authentication
source_filename: super-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: First-party sources only — github.com/super-studio/ecforce_headless (src/lib/ecforce-sdk/shared/index.ts, src/env.js), the READMEs of\n  @super_studio/ecforce-ai-agent-server and @super_studio/ecforce-ai-agent-react on registry.npmjs.org, and the anonymously served RFC 8414 metadata\n  at agent.ec-force.com.\nnote: 'derive-authentication.py was not run: it derives from openapi/, and no OpenAPI is published for any SUPER STUDIO API. Everything below\n  is quoted from code and documentation SUPER STUDIO published itself. Three different APIs use three different schemes.'\napis:\n- api: ecforce API v2\n  schemes:\n  - id: ecforce_admin_token\n    type: apiKey\n    in: header\n    name: Authorization\n    format: Token token=\"<access token>\"\n    description: Rails-style token authentication. The token belongs to an \"API connection user\" created in the ecforce admin under システム管理 > メンバー管理\n      (System Admin > Member Management);\
  \ the access token and the API login password are shown once, immediately after issuance, and cannot be\n      re-read afterwards. The API connection option is a paid contract add-on.\n    evidence: &id001\n      file: src/lib/ecforce-sdk/shared/index.ts\n      repo: https://github.com/super-studio/ecforce_headless\n      quote: 'Authorization: `Token token=\"${env.ECF_API_TOKEN}\"`'\n  - id: ecforce_customer_session\n    type: http\n    scheme: session\n    description: v2/customer authenticates as a shopper. The first-party headless sample signs in with POST /customers/sign_in and carries the\n      resulting session for My Page-equivalent calls.\n    evidence: &id002\n      file: src/lib/ecforce-sdk/customer/session/endpoints.ts\n      repo: https://github.com/super-studio/ecforce_headless\n  content_type: application/json\n  transport_note: Base host is per-merchant and merchant-configurable — integration guides show the form https://api.<shop-domain> and note the\n    \"api\" label\
  \ may differ per shop. There is no single shared ecforce API host.\n- api: ecforce AI Agent API\n  schemes:\n  - id: ai_agent_api_key\n    type: apiKey\n    in: header\n    name: unspecified\n    description: An API key issued in the ecforce admin screens, supplied to the first-party server SDK as the AI_AGENT_API_KEY environment variable.\n      The SDK sets the header internally and the published README does not name it, so the header name is recorded as unspecified rather than\n      guessed.\n    evidence: &id003\n      package: '@super_studio/ecforce-ai-agent-server'\n      version: 1.5.0\n      quote: '`AI_AGENT_API_KEY`: 必須。管理画面で発行した API キー'\n  - id: agent_session_token\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: Short-lived chat session tokens minted server-side by client.internalChat.createSession() and handed to the browser components.\n      Shape is { token, expiresAt }. The SDK depends on jose and @panva/hkdf, so these are signed/derived tokens\
  \ rather than opaque strings.\n  - id: mcp_token_secret\n    type: apiKey\n    in: header\n    name: unspecified\n    description: MCP_TOKEN_SECRET signs and verifies MCP tokens when a tenant application exposes its own MCP tools alongside ecforce's. Required\n      only when implementing MCP.\n- api: ecforce AI MCP\n  schemes:\n  - id: mcp_oauth\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    authorization_url: https://agent.ec-force.com/mcp/oauth/authorize\n    token_url: https://agent.ec-force.com/mcp/oauth/token\n    revocation_url: https://agent.ec-force.com/mcp/oauth/revoke\n    registration_url: https://agent.ec-force.com/mcp/oauth/register\n    scopes: &id004\n    - mcp\n    token_endpoint_auth_methods: &id005\n    - none\n    description: 'Public-client OAuth 2.1-shaped flow: no client secret, PKCE S256 mandatory, RFC 7591 dynamic client registration open to anonymous\n      callers, refresh tokens supported. This is the pattern an MCP client is expected to\
  \ complete on its own with no pre-registration.'\n    evidence: &id006\n      url: https://agent.ec-force.com/.well-known/oauth-authorization-server\n      status: 200\nmfa:\n  available: true\n  scope: ecforce administrator accounts\n  source: https://ec-force.com/security\n  note: Two-factor authentication and IP-address restriction are offered for admin access.\nschemes:\n- id: ecforce_admin_token\n  type: apiKey\n  in: header\n  name: Authorization\n  format: Token token=\"<access token>\"\n  description: Rails-style token authentication. The token belongs to an \"API connection user\" created in the ecforce admin under システム管理 > メンバー管理\n    (System Admin > Member Management); the access token and the API login password are shown once, immediately after issuance, and cannot be\n    re-read afterwards. The API connection option is a paid contract add-on.\n  evidence: *id001\n  api: ecforce API v2\n- id: ecforce_customer_session\n  type: http\n  scheme: session\n  description: v2/customer\
  \ authenticates as a shopper. The first-party headless sample signs in with POST /customers/sign_in and carries the resulting\n    session for My Page-equivalent calls.\n  evidence: *id002\n  api: ecforce API v2\n- id: ai_agent_api_key\n  type: apiKey\n  in: header\n  name: unspecified\n  description: An API key issued in the ecforce admin screens, supplied to the first-party server SDK as the AI_AGENT_API_KEY environment variable.\n    The SDK sets the header internally and the published README does not name it, so the header name is recorded as unspecified rather than guessed.\n  evidence: *id003\n  api: ecforce AI Agent API\n- id: agent_session_token\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: Short-lived chat session tokens minted server-side by client.internalChat.createSession() and handed to the browser components.\n    Shape is { token, expiresAt }. The SDK depends on jose and @panva/hkdf, so these are signed/derived tokens rather than opaque strings.\n\
  \  api: ecforce AI Agent API\n- id: mcp_token_secret\n  type: apiKey\n  in: header\n  name: unspecified\n  description: MCP_TOKEN_SECRET signs and verifies MCP tokens when a tenant application exposes its own MCP tools alongside ecforce's. Required\n    only when implementing MCP.\n  api: ecforce AI Agent API\n- id: mcp_oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_url: https://agent.ec-force.com/mcp/oauth/authorize\n  token_url: https://agent.ec-force.com/mcp/oauth/token\n  revocation_url: https://agent.ec-force.com/mcp/oauth/revoke\n  registration_url: https://agent.ec-force.com/mcp/oauth/register\n  scopes: *id004\n  token_endpoint_auth_methods: *id005\n  description: 'Public-client OAuth 2.1-shaped flow: no client secret, PKCE S256 mandatory, RFC 7591 dynamic client registration open to anonymous\n    callers, refresh tokens supported. This is the pattern an MCP client is expected to complete on its own with no pre-registration.'\n  evidence: *id006\n\
  \  api: ecforce AI MCP\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-studio/refs/heads/main/authentication/super-studio-authentication.yml
summary_line: 6 schemes
tags:
- Company
- E-Commerce
- Commerce
- Subscription Commerce
- Order Management
- Marketing Automation
- Business Intelligence
- Software-as-a-Service
- Artificial Intelligence
- Agents
- MCP
- Japan
---
