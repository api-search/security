---
api_key_in:
- header
api_specs:
- filename: karumi-analytics-api-openapi.yml
  format: yaml
  label: Karumi Analytics API
  slug: karumi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-analytics-api-openapi.yml
- filename: karumi-sessions-api-openapi.yml
  format: yaml
  label: Karumi Sessions API
  slug: karumi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-sessions-api-openapi.yml
- filename: karumi-targets-api-openapi.yml
  format: yaml
  label: Karumi Targets API
  slug: karumi-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-targets-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Karumi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Karumi secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Karumi
provider_slug: karumi
scheme_count: 2
schemes:
- applies_to: Karumi Public API (https://api.karumi.ai/api/v1)
  in: header
  key_management: Organization API keys are created and revoked from the Karumi workspace; the MCP server exposes list_api_keys, create_api_key and revoke_api_key tools for the same lifecycle.
  name: X-Api-Key
  note: 'The spec does NOT declare this in components.securitySchemes. It is modelled as an optional (required:false) `x-api-key` header parameter on all nine operations, with the requirement stated in prose in info.description. The API in fact rejects unauthenticated calls with HTTP 401. This is a real spec defect worth reporting to the provider: a machine reading securitySchemes alone would conclude the API is open. overlays/karumi-public-api-overlay.yaml records the corrected security model without mutating the harvested spec.'
  parameter_name: x-api-key
  scope: organization
  sources:
  - openapi/karumi-public-api-openapi.json
  type: apiKey
- applies_to: Karumi MCP Server (https://api.karumi.ai/mcp/)
  authorization_server: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1
  bearer_methods:
  - header
  dynamic_client_registration: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/clients/register
  flows:
  - authorizationUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    pkce: true
    pkce_methods:
    - S256
    - plain
    scopes:
    - openid
    - profile
    - email
    - phone
    - offline_access
    tokenUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token
  name: OAuth2
  note: Karumi delegates MCP authorization to its Supabase Auth project rather than running its own authorization server, so the RFC 8414 metadata is served from supabase.co and the scopes are Supabase's OIDC set, not Karumi-specific permissions. Karumi's own documentation describes the flow as "OAuth 2.0 (authorization-code flow over HTTPS) with explicit user consent" and says access is scoped to the organizations the authenticating user belongs to — that organization scoping is enforced server-side, not expressed as an OAuth scope.
  protected_resource_metadata: https://api.karumi.ai/.well-known/oauth-protected-resource
  sources:
  - well-known/karumi-oauth-protected-resource.json
  - well-known/karumi-oauth-authorization-server.json
  type: oauth2
slug: karumi-authentication
source_filename: karumi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/karumi-public-api-openapi.json\ndocs: https://www.karumi.ai/mcp-documentation\nevidence:\n- url: https://api.karumi.ai/api/v1/openapi.json\n  http_status: 200\n  note: info.description states \"Authenticate using the X-Api-Key header with your\n    organization's API key.\"\n- url: https://api.karumi.ai/api/v1/sessions\n  http_status: 401\n  note: 'Unauthenticated GET returns {\"detail\":\"Missing X-Api-Key header\"} — the\n    key requirement was observed live, not only read from the spec.'\n- url: https://api.karumi.ai/mcp/\n  http_status: 401\n  note: 'Unauthenticated MCP tools/list returns {\"error\": \"unauthorized\"} with\n    WWW-Authenticate: Bearer resource_metadata=\"https://api.karumi.ai/.well-known/oauth-protected-resource\"\n    — a correct RFC 9728 challenge.'\n- url: https://api.karumi.ai/.well-known/oauth-protected-resource\n  http_status: 200\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n\
  \  - header\n  oauth2_flows:\n  - authorizationCode\n  surfaces: 2\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to: Karumi Public API (https://api.karumi.ai/api/v1)\n  scope: organization\n  sources:\n  - openapi/karumi-public-api-openapi.json\n  note: >-\n    The spec does NOT declare this in components.securitySchemes. It is modelled as an\n    optional (required:false) `x-api-key` header parameter on all nine operations, with\n    the requirement stated in prose in info.description. The API in fact rejects\n    unauthenticated calls with HTTP 401. This is a real spec defect worth reporting to the\n    provider: a machine reading securitySchemes alone would conclude the API is open.\n    overlays/karumi-public-api-overlay.yaml records the corrected security model without\n    mutating the harvested spec.\n  key_management: >-\n    Organization API keys are created and revoked from the Karumi workspace; the MCP\n    server exposes\
  \ list_api_keys, create_api_key and revoke_api_key tools for the same\n    lifecycle.\n- name: OAuth2\n  type: oauth2\n  applies_to: Karumi MCP Server (https://api.karumi.ai/mcp/)\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    pkce_methods:\n    - S256\n    - plain\n    authorizationUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token\n    scopes:\n    - openid\n    - profile\n    - email\n    - phone\n    - offline_access\n  bearer_methods:\n  - header\n  dynamic_client_registration: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/clients/register\n  protected_resource_metadata: https://api.karumi.ai/.well-known/oauth-protected-resource\n  authorization_server: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1\n  sources:\n  - well-known/karumi-oauth-protected-resource.json\n  - well-known/karumi-oauth-authorization-server.json\n  note: >-\n    Karumi delegates MCP authorization\
  \ to its Supabase Auth project rather than running\n    its own authorization server, so the RFC 8414 metadata is served from supabase.co and\n    the scopes are Supabase's OIDC set, not Karumi-specific permissions. Karumi's own\n    documentation describes the flow as \"OAuth 2.0 (authorization-code flow over HTTPS)\n    with explicit user consent\" and says access is scoped to the organizations the\n    authenticating user belongs to — that organization scoping is enforced server-side,\n    not expressed as an OAuth scope.\nrevocation:\n  user: Karumi account settings (disconnect the connector or revoke access)\n  source: https://www.karumi.ai/mcp-documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/authentication/karumi-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- AI Agents
- Product Demos
- Sales Enablement
- Go-To-Market
- Software-as-a-Service
- Conversational AI
- Video
- Y Combinator
- MCP
- agent-native
- Analytics
- Conversation Intelligence
---
