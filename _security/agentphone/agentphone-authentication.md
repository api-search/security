---
api_key_in:
- header
api_specs:
- filename: agentphone-openapi-original.json
  format: json
  label: AgentPhone API
  slug: agentphone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-openapi-original.json
auth_types:
- http
- oauth2
description: 'The AgentPhone REST API authenticates with an API key passed as an HTTP Bearer token on every request (Authorization: Bearer <API_KEY>). Keys are created in the dashboard under Settings -> API Keys. A separate OAuth 2.0 authorization server (advertised at /.well-known/oauth-authorization-server and /.well-known/openid-configuration on api.agentphone.ai) secures the remote MCP surface with authorization_code + PKCE, dynamic client registration, refresh tokens, and a single `mcp` scope.'
kind: authentication
layout: security
method: searched
name: Agentphone Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AgentPhone secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AgentPhone
provider_slug: agentphone
scheme_count: 2
schemes:
- description: API key supplied as a Bearer token on every REST request.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/agentphone-openapi-original.json
  type: http
- description: OAuth 2.0 / OIDC authorization server protecting the remote MCP surface (RFC 8414 metadata). Not used by the core REST API.
  flows:
  - authorizationUrl: https://agentphone.ai/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://api.agentphone.ai/oauth/register
    revocationUrl: https://api.agentphone.ai/oauth/revoke
    scopes:
      mcp: Access the AgentPhone MCP tools
    tokenUrl: https://api.agentphone.ai/oauth/token
  name: MCPOAuth2
  pkce: true
  sources:
  - well-known/agentphone-oauth-authorization-server.json
  type: oauth2
slug: agentphone-authentication
source_filename: agentphone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/agentphone-openapi-original.json\ndocs: https://docs.agentphone.ai/welcome\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\ndescription: >-\n  The AgentPhone REST API authenticates with an API key passed as an HTTP\n  Bearer token on every request (Authorization: Bearer <API_KEY>). Keys are\n  created in the dashboard under Settings -> API Keys. A separate OAuth 2.0\n  authorization server (advertised at /.well-known/oauth-authorization-server\n  and /.well-known/openid-configuration on api.agentphone.ai) secures the\n  remote MCP surface with authorization_code + PKCE, dynamic client\n  registration, refresh tokens, and a single `mcp` scope.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: API key supplied as a Bearer token on every REST request.\n  sources:\n  - openapi/agentphone-openapi-original.json\n- name: MCPOAuth2\n  type:\
  \ oauth2\n  description: >-\n    OAuth 2.0 / OIDC authorization server protecting the remote MCP surface\n    (RFC 8414 metadata). Not used by the core REST API.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://agentphone.ai/oauth/authorize\n    tokenUrl: https://api.agentphone.ai/oauth/token\n    registrationUrl: https://api.agentphone.ai/oauth/register\n    revocationUrl: https://api.agentphone.ai/oauth/revoke\n    scopes:\n      mcp: Access the AgentPhone MCP tools\n  pkce: true\n  sources:\n  - well-known/agentphone-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/authentication/agentphone-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Telephony
- Phone Numbers
- SMS
- Voice
- AI Agents
- Messaging
- Communications
- Webhooks
- MCP
- iMessage
---
