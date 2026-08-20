---
api_key_in:
- header
api_specs:
- filename: agentphone-agent-webhooks-api-openapi.yml
  format: yaml
  label: AgentPhone agent-webhooks API
  slug: agentphone-agent-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-agent-webhooks-api-openapi.yml
- filename: agentphone-agents-api-openapi.yml
  format: yaml
  label: AgentPhone agents API
  slug: agentphone-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-agents-api-openapi.yml
- filename: agentphone-calls-api-openapi.yml
  format: yaml
  label: AgentPhone calls API
  slug: agentphone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-calls-api-openapi.yml
- filename: agentphone-contactcards-api-openapi.yml
  format: yaml
  label: AgentPhone contactCards API
  slug: agentphone-contactcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-contactcards-api-openapi.yml
- filename: agentphone-contacts-api-openapi.yml
  format: yaml
  label: AgentPhone contacts API
  slug: agentphone-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-contacts-api-openapi.yml
- filename: agentphone-conversations-api-openapi.yml
  format: yaml
  label: AgentPhone conversations API
  slug: agentphone-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-conversations-api-openapi.yml
- filename: agentphone-location-api-openapi.yml
  format: yaml
  label: AgentPhone location API
  slug: agentphone-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-location-api-openapi.yml
- filename: agentphone-messages-api-openapi.yml
  format: yaml
  label: AgentPhone messages API
  slug: agentphone-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-messages-api-openapi.yml
- filename: agentphone-numbers-api-openapi.yml
  format: yaml
  label: AgentPhone numbers API
  slug: agentphone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-numbers-api-openapi.yml
- filename: agentphone-registration-api-openapi.yml
  format: yaml
  label: AgentPhone registration API
  slug: agentphone-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-registration-api-openapi.yml
- filename: agentphone-sub-accounts-api-openapi.yml
  format: yaml
  label: AgentPhone sub-accounts API
  slug: agentphone-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-sub-accounts-api-openapi.yml
- filename: agentphone-usage-api-openapi.yml
  format: yaml
  label: AgentPhone usage API
  slug: agentphone-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-usage-api-openapi.yml
- filename: agentphone-webhooks-api-openapi.yml
  format: yaml
  label: AgentPhone webhooks API
  slug: agentphone-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-webhooks-api-openapi.yml
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
- Webhook
- MCP
- iMessage
---
