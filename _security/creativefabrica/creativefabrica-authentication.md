---
anonymous_access: false
api_key_in: []
api_specs:
- filename: creativefabrica-generations-api-openapi.yml
  format: yaml
  label: Creative Fabrica Generations API
  slug: creativefabrica-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-generations-api-openapi.yml
- filename: creativefabrica-models-api-openapi.yml
  format: yaml
  label: Creative Fabrica Models API
  slug: creativefabrica-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-models-api-openapi.yml
- filename: creativefabrica-presets-api-openapi.yml
  format: yaml
  label: Creative Fabrica Presets API
  slug: creativefabrica-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-presets-api-openapi.yml
- filename: creativefabrica-voices-api-openapi.yml
  format: yaml
  label: Creative Fabrica Voices API
  slug: creativefabrica-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-voices-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Creative Fabrica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creative Fabrica secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Creative Fabrica
provider_slug: creativefabrica
scheme_count: 2
schemes:
- applies_to: https://api.idea.ai/genai/v1
  bearerFormat: API key
  description: 'idea.ai GenAI API key (`sk-...`). Sent as `Authorization: Bearer sk-...`. One bearer key per API team; setup is free and the key is generated instantly through the self-serve flow at https://www.idea.ai/platform/get-api-key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/creativefabrica-idea-ai-genai-openapi.yml
  - https://www.idea.ai/platform/get-api-key
  surface: openapi/creativefabrica-idea-ai-genai-openapi.yml
  type: http
- authorization_endpoint: https://oauth.creativefabrica.com/oauth2/auth
  authorization_server_metadata: https://oauth.creativefabrica.com/.well-known/oauth-authorization-server
  description: 'Remote MCP server (https://mcp.idea.ai/mcp) requires OAuth 2.1 sign-in. Authorization server: https://oauth.creativefabrica.com. Dynamic client registration is enabled; the user authorises an idea.ai account and the access token is scoped to MCP tool calls.'
  flow: authorization_code_pkce
  name: oauth21-mcp
  pkce: S256
  protected_resource_metadata: https://mcp.idea.ai/.well-known/oauth-protected-resource
  registration_endpoint: https://oauth.creativefabrica.com/oauth2/register
  scheme_name: OAuth 2.1
  scopes:
  - openid
  - email
  - mcp:read
  - mcp:generate
  sources:
  - mcp/creativefabrica-mcp.yml
  - https://mcp.idea.ai/.well-known/oauth-protected-resource
  surface: https://mcp.idea.ai/mcp
  token_endpoint: https://oauth.creativefabrica.com/oauth2/token
  type: oauth2
slug: creativefabrica-authentication
source_filename: creativefabrica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n  - openapi/creativefabrica-idea-ai-genai-openapi.yml\n  - https://www.idea.ai/platform/docs\n  - https://www.idea.ai/platform/get-api-key\n  - https://www.idea.ai/mcp/docs\n  - https://mcp.idea.ai/.well-known/oauth-protected-resource\n  - https://oauth.creativefabrica.com/.well-known/oauth-authorization-server\ndocs: https://www.idea.ai/platform/get-api-key\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: >-\n    idea.ai GenAI API key (`sk-...`). Sent as `Authorization: Bearer sk-...`.\n    One bearer key per API team; setup is free and the key is generated\n    instantly through the self-serve flow at\n    https://www.idea.ai/platform/get-api-key.\n  surface: openapi/creativefabrica-idea-ai-genai-openapi.yml\n  applies_to: https://api.idea.ai/genai/v1\n  sources:\n  - openapi/creativefabrica-idea-ai-genai-openapi.yml\n  - https://www.idea.ai/platform/get-api-key\n\
  - name: oauth21-mcp\n  type: oauth2\n  flow: authorization_code_pkce\n  scheme_name: OAuth 2.1\n  description: >-\n    Remote MCP server (https://mcp.idea.ai/mcp) requires OAuth 2.1 sign-in.\n    Authorization server: https://oauth.creativefabrica.com. Dynamic client\n    registration is enabled; the user authorises an idea.ai account and the\n    access token is scoped to MCP tool calls.\n  surface: https://mcp.idea.ai/mcp\n  scopes:\n  - openid\n  - email\n  - mcp:read\n  - mcp:generate\n  pkce: S256\n  authorization_endpoint: https://oauth.creativefabrica.com/oauth2/auth\n  token_endpoint: https://oauth.creativefabrica.com/oauth2/token\n  registration_endpoint: https://oauth.creativefabrica.com/oauth2/register\n  protected_resource_metadata: https://mcp.idea.ai/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://oauth.creativefabrica.com/.well-known/oauth-authorization-server\n  sources:\n  - mcp/creativefabrica-mcp.yml\n  - https://mcp.idea.ai/.well-known/oauth-protected-resource\n\
  notes: >-\n  The idea.ai GenAI REST API and the idea.ai MCP server use different\n  auth: REST = static bearer `sk-...` key; MCP = OAuth 2.1 with the four\n  scopes above. The 401 path on REST returns an RFC 9457 problem with\n  `code: unauthenticated` or `code: forbidden`; see\n  errors/creativefabrica-problem-types.yml.\n"
source_yaml_url: https://artifacts.apis.io/creativefabrica/authentication/creativefabrica-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Creative Marketplace
- Digital Assets
- Fonts
- Graphics
- Print on Demand
- Embroidery
- Design Tools
- Subscription Service
- Amsterdam
---
