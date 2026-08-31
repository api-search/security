---
api_key_in: []
api_specs:
- filename: samaya-ai-organizations-api-openapi.yml
  format: yaml
  label: Samaya AI Organizations API
  slug: samaya-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-organizations-api-openapi.yml
- filename: samaya-ai-teams-api-openapi.yml
  format: yaml
  label: Samaya AI Teams API
  slug: samaya-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-teams-api-openapi.yml
- filename: samaya-ai-users-api-openapi.yml
  format: yaml
  label: Samaya AI Users API
  slug: samaya-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Samaya Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Samaya AI secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Samaya AI
provider_slug: samaya-ai
scheme_count: 3
schemes:
- applies_to: https://api.samaya.ai
  description: HTTP bearer token issued by WorkOS as a machine-to-machine credential. Declared in the published OpenAPI as the only securityScheme and applied to all six operations.
  method: derived
  name: WorkOsM2MAuth
  scheme: bearer
  sources:
  - openapi/samaya-ai-public-api-openapi.json
  surface: Samaya Public API
  type: http
- applies_to: https://mcp.samaya.ai/mcp
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.1 authorization-code flow with PKCE. An anonymous JSON-RPC tools/list POST returns HTTP 401 with WWW-Authenticate Bearer error="invalid_token" and resource_metadata="https://mcp.samaya.ai/.well-known/oauth-protected-resource/mcp".
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.samaya.ai/authorize
      refreshUrl: https://mcp.samaya.ai/token
      scopes: {}
      tokenUrl: https://mcp.samaya.ai/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.samaya.ai/
  method: probed
  name: MCPOAuth
  registration_endpoint: https://mcp.samaya.ai/register
  revocation_endpoint: https://mcp.samaya.ai/revoke
  sources:
  - well-known/samaya-ai-oauth-authorization-server.json
  - well-known/samaya-ai-oauth-protected-resource.json
  surface: Samaya MCP Server
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to: https://api.samaya.ai/graphql/
  description: Anonymous POST of the introspection query returns HTTP 401 with the plain-text body "Unauthorized". The credential type is not advertised anonymously; access-control-allow-origin is pinned to https://app.samaya.ai, indicating a browser-session-scoped app surface.
  evidence:
    body: Unauthorized
    http_status: 401
    url: https://api.samaya.ai/graphql/
  method: probed
  name: GraphQLSessionAuth
  surface: Samaya GraphQL API
  type: unknown
slug: samaya-ai-authentication
source_filename: samaya-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  openapi/samaya-ai-public-api-openapi.json (derived) plus live probes of\n  https://mcp.samaya.ai/mcp, https://mcp.samaya.ai/.well-known/oauth-authorization-server,\n  https://mcp.samaya.ai/.well-known/oauth-protected-resource/mcp and https://api.samaya.ai/graphql/\nsummary:\n  types:\n  - http\n  - oauth2\n  surfaces: 3\n  note: >-\n    Two distinct authentication models. The REST provisioning API uses a WorkOS\n    machine-to-machine bearer token. The remote MCP server uses full OAuth 2.1 with dynamic\n    client registration and PKCE, advertised via RFC 9728 protected-resource metadata.\nschemes:\n- name: WorkOsM2MAuth\n  type: http\n  scheme: bearer\n  surface: Samaya Public API\n  applies_to: https://api.samaya.ai\n  description: >-\n    HTTP bearer token issued by WorkOS as a machine-to-machine credential. Declared in the\n    published OpenAPI as the only securityScheme and applied to all six operations.\n  sources:\n\
  \  - openapi/samaya-ai-public-api-openapi.json\n  method: derived\n- name: MCPOAuth\n  type: oauth2\n  surface: Samaya MCP Server\n  applies_to: https://mcp.samaya.ai/mcp\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE. An anonymous JSON-RPC tools/list POST returns\n    HTTP 401 with WWW-Authenticate Bearer error=\"invalid_token\" and\n    resource_metadata=\"https://mcp.samaya.ai/.well-known/oauth-protected-resource/mcp\".\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.samaya.ai/authorize\n      tokenUrl: https://mcp.samaya.ai/token\n      refreshUrl: https://mcp.samaya.ai/token\n      scopes: {}\n  registration_endpoint: https://mcp.samaya.ai/register\n  revocation_endpoint: https://mcp.samaya.ai/revoke\n  issuer: https://mcp.samaya.ai/\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n\
  \  bearer_methods_supported:\n  - header\n  dynamic_client_registration: true\n  sources:\n  - well-known/samaya-ai-oauth-authorization-server.json\n  - well-known/samaya-ai-oauth-protected-resource.json\n  method: probed\n- name: GraphQLSessionAuth\n  type: unknown\n  surface: Samaya GraphQL API\n  applies_to: https://api.samaya.ai/graphql/\n  description: >-\n    Anonymous POST of the introspection query returns HTTP 401 with the plain-text body\n    \"Unauthorized\". The credential type is not advertised anonymously; access-control-allow-origin\n    is pinned to https://app.samaya.ai, indicating a browser-session-scoped app surface.\n  method: probed\n  evidence:\n    url: https://api.samaya.ai/graphql/\n    http_status: 401\n    body: Unauthorized\ndocs: null\ndocs_note: >-\n  Samaya publishes no public authentication documentation page. The auth model above was read\n  entirely from the machine-readable surfaces the company serves.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/authentication/samaya-ai-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- artificial-intelligence
- Financial-Services
- investment-research
- AI Agents
- MCP
- agent-native
- capital-markets
- enterprise-search
- retrieval
- graphql
---
