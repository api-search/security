---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corebee-ai-auth-api-openapi.yml
  format: yaml
  label: Corebee Auth API
  slug: corebee-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-auth-api-openapi.yml
- filename: corebee-ai-contacts-api-openapi.yml
  format: yaml
  label: Corebee Contacts API
  slug: corebee-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-contacts-api-openapi.yml
- filename: corebee-ai-conversations-api-openapi.yml
  format: yaml
  label: Corebee Conversations API
  slug: corebee-ai-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-conversations-api-openapi.yml
- filename: corebee-ai-labels-api-openapi.yml
  format: yaml
  label: Corebee Labels API
  slug: corebee-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-labels-api-openapi.yml
- filename: corebee-ai-voice-api-openapi.yml
  format: yaml
  label: Corebee Voice API
  slug: corebee-ai-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-voice-api-openapi.yml
- filename: corebee-ai-webhooks-api-openapi.yml
  format: yaml
  label: Corebee Webhooks API
  slug: corebee-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Corebee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corebee secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corebee
provider_slug: corebee-ai
scheme_count: 2
schemes:
- description: Org-scoped API key, or an OAuth 2.1 access token (authorization_code + PKCE; see /.well-known/oauth-protected-resource). An API key is minted in the Corebee dashboard under Settings, Developers, API keys, and the SCOPES it carries are chosen at that moment and cannot be widened afterwards. Every voice/bridge operation needs the voice:bridge scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/corebee-ai-openapi.yml
  type: http
- description: OAuth 2.1 with Dynamic Client Registration, documented in llms.txt ("Authentication is OAuth 2.1 (with Dynamic Client Registration) or an org-scoped API key") and published as RFC 8414 authorization-server metadata. Discovery documents were read; no token or authorization endpoint was called.
  flows:
    authorizationCode:
      authorizationUrl: https://corebee.ai/api/v1/mcp/oauth/authorize
      pkce: S256
      tokenUrl: https://corebee.ai/api/v1/mcp/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  metadata:
  - https://corebee.ai/.well-known/oauth-authorization-server
  - https://corebee.ai/.well-known/oauth-protected-resource
  name: oauth2.1
  registration_endpoint: https://corebee.ai/api/v1/mcp/oauth/register
  scopes: scopes/corebee-ai-scopes.yml
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: corebee-ai-authentication
source_filename: corebee-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corebee.ai/api/v1/openapi.json\ndocs: https://corebee.ai/llms.txt\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Org-scoped API key, or an OAuth 2.1 access token (authorization_code + PKCE; see\n    /.well-known/oauth-protected-resource). An API key is minted in the Corebee dashboard under\n    Settings, Developers, API keys, and the SCOPES it carries are chosen at that moment and cannot\n    be widened afterwards. Every voice/bridge operation needs the voice:bridge scope.\n  sources:\n  - openapi/corebee-ai-openapi.yml\n- name: oauth2.1\n  type: oauth2\n  description: OAuth 2.1 with Dynamic Client Registration, documented in llms.txt (\"Authentication\n    is OAuth 2.1 (with Dynamic Client Registration) or an org-scoped API key\") and published as\n    RFC 8414 authorization-server metadata. Discovery documents were read; no token or\n    authorization\
  \ endpoint was called.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://corebee.ai/api/v1/mcp/oauth/authorize\n      tokenUrl: https://corebee.ai/api/v1/mcp/oauth/token\n      pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  registration_endpoint: https://corebee.ai/api/v1/mcp/oauth/register\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  metadata:\n  - https://corebee.ai/.well-known/oauth-authorization-server\n  - https://corebee.ai/.well-known/oauth-protected-resource\n  scopes: scopes/corebee-ai-scopes.yml\nlegacy_docs_note: The HTML page https://corebee.ai/docs/api still says requests authenticate via a\n  \"Supabase JWT token\" against /api/inbox/* paths; the v1 OpenAPI (https://corebee.ai/api/v1) is the\n  current contract.\n"
source_yaml_url: https://artifacts.apis.io/corebee-ai/authentication/corebee-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Customer Service
- Artificial Intelligence
- Chatbots
- Help Desk
- Omnichannel Messaging
- Voice Agents
- MCP
---
