---
api_key_in: []
api_specs:
- filename: gojiberry-ai-appexternal-api-openapi.yml
  format: yaml
  label: Gojiberry AI AppExternal API
  slug: gojiberry-ai-appexternal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-appexternal-api-openapi.yml
- filename: gojiberry-ai-campaigns-api-openapi.yml
  format: yaml
  label: Gojiberry AI Campaigns API
  slug: gojiberry-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-campaigns-api-openapi.yml
- filename: gojiberry-ai-contacts-api-openapi.yml
  format: yaml
  label: Gojiberry AI Contacts API
  slug: gojiberry-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-contacts-api-openapi.yml
- filename: gojiberry-ai-lead-source-agents-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lead source agents API
  slug: gojiberry-ai-lead-source-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
- filename: gojiberry-ai-lists-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lists API
  slug: gojiberry-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lists-api-openapi.yml
- filename: gojiberry-ai-organization-api-openapi.yml
  format: yaml
  label: Gojiberry AI Organization API
  slug: gojiberry-ai-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-organization-api-openapi.yml
- filename: gojiberry-ai-unibox-api-openapi.yml
  format: yaml
  label: Gojiberry AI Unibox API
  slug: gojiberry-ai-unibox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-unibox-api-openapi.yml
- filename: gojiberry-ai-user-api-openapi.yml
  format: yaml
  label: Gojiberry AI User API
  slug: gojiberry-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gojiberry Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gojiberry AI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Enter API Key
  name: API-Key
  scheme: bearer
  sources:
  - openapi/gojiberry-ai-appexternal-api-openapi.yml
  - openapi/gojiberry-ai-campaigns-api-openapi.yml
  - openapi/gojiberry-ai-contacts-api-openapi.yml
  - openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
  - openapi/gojiberry-ai-lists-api-openapi.yml
  - openapi/gojiberry-ai-organization-api-openapi.yml
  - openapi/gojiberry-ai-unibox-api-openapi.yml
  - openapi/gojiberry-ai-user-api-openapi.yml
  surface: rest
  type: http
- description: Hosted MCP server authorization, discovered anonymously from RFC 8414 authorization server metadata and RFC 9728 protected resource metadata.
  flows:
  - authorizationUrl: https://mcp.gojiberry.ai/authorize
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://mcp.gojiberry.ai/register
    scopes:
    - mcp:tools
    - claudeai
    tokenUrl: https://mcp.gojiberry.ai/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  name: MCP OAuth 2.1
  see: scopes/gojiberry-ai-scopes.yml
  sources:
  - well-known/gojiberry-ai-oauth-authorization-server.json
  - well-known/gojiberry-ai-oauth-protected-resource.json
  surface: mcp
  type: oauth2
slug: gojiberry-ai-authentication
source_filename: gojiberry-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://ext.gojiberry.ai/documentation\nsource: openapi/gojiberry-ai-appexternal-api-openapi.yml, openapi/gojiberry-ai-campaigns-api-openapi.yml,\n  openapi/gojiberry-ai-contacts-api-openapi.yml, openapi/gojiberry-ai-lead-source-agents-api-openapi.yml,\n  openapi/gojiberry-ai-lists-api-openapi.yml, openapi/gojiberry-ai-organization-api-openapi.yml,\n  openapi/gojiberry-ai-unibox-api-openapi.yml, openapi/gojiberry-ai-user-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  note: >-\n    Two distinct auth surfaces. The REST External API (ext.gojiberry.ai) uses a\n    bearer API key (JWT) issued in-app; the hosted MCP server (mcp.gojiberry.ai)\n    uses OAuth 2.1 authorization code + PKCE with dynamic client registration.\n  oauth2_flows: [authorizationCode]\n  surfaces: [rest, mcp]\nprovisioning:\n  rest_api_key:\n    steps:\n    - Log in at https://app.gojiberry.ai\n    - Navigate to Settings -> API\n    - Click \"Create\
  \ API Key\"\n    - Copy the key (shown once)\n    - 'Send it as: Authorization: Bearer YOUR_API_KEY'\n    docs: https://ext.gojiberry.ai/documentation\nimpersonation:\n  supported: true\n  header: x-impersonate-user-id\n  rule: >-\n    The API key must belong to the organization OWNER and the impersonated user\n    must belong to the same organization; violations return 401. Present as an\n    optional header parameter on every External API operation.\n  helpers: [GET /v1/organization/members, GET /v1/user/me]\nschemes:\n- name: API-Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter API Key\n  surface: rest\n  sources:\n  - openapi/gojiberry-ai-appexternal-api-openapi.yml\n  - openapi/gojiberry-ai-campaigns-api-openapi.yml\n  - openapi/gojiberry-ai-contacts-api-openapi.yml\n  - openapi/gojiberry-ai-lead-source-agents-api-openapi.yml\n  - openapi/gojiberry-ai-lists-api-openapi.yml\n  - openapi/gojiberry-ai-organization-api-openapi.yml\n  - openapi/gojiberry-ai-unibox-api-openapi.yml\n\
  \  - openapi/gojiberry-ai-user-api-openapi.yml\n- name: MCP OAuth 2.1\n  type: oauth2\n  surface: mcp\n  description: >-\n    Hosted MCP server authorization, discovered anonymously from RFC 8414\n    authorization server metadata and RFC 9728 protected resource metadata.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.gojiberry.ai/authorize\n    tokenUrl: https://mcp.gojiberry.ai/token\n    registrationUrl: https://mcp.gojiberry.ai/register\n    code_challenge_methods: [S256, plain]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post]\n    scopes: [mcp:tools, claudeai]\n  sources:\n  - well-known/gojiberry-ai-oauth-authorization-server.json\n  - well-known/gojiberry-ai-oauth-protected-resource.json\n  see: scopes/gojiberry-ai-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/authentication/gojiberry-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
---
