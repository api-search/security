---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coupondroid-es-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid España A2a API
  slug: coupondroid-es-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-a2a-api-openapi.yml
- filename: coupondroid-es-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid España Auth.md API
  slug: coupondroid-es-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-auth-md-api-openapi.yml
- filename: coupondroid-es-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid España Llms.txt API
  slug: coupondroid-es-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-llms-txt-api-openapi.yml
- filename: coupondroid-es-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid España MCP API
  slug: coupondroid-es-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-mcp-api-openapi.yml
- filename: coupondroid-es-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid España .well Known API
  slug: coupondroid-es-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid España Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid España secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid España
provider_slug: coupondroid-es
scheme_count: 1
schemes:
- applies_to:
  - managementMcp
  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  discovery:
  - https://coupondroid.es/.well-known/oauth-protected-resource
  - https://coupondroid.es/.well-known/oauth-authorization-server
  dynamic_client_registration: https://coupondroid.es/oauth/register
  flows:
  - authorizationUrl: https://coupondroid.es/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://coupondroid.es/oauth/token
  name: oauth2
  pkce: S256 only
  refresh: grant_type=refresh_token
  revocation_url: https://coupondroid.es/oauth/revoke
  sources:
  - openapi/coupondroid-es-openapi.yml
  - https://coupondroid.es/auth.md
  token_placement: 'Authorization: Bearer header'
  type: oauth2
slug: coupondroid-es-authentication
source_filename: coupondroid-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.es/auth.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.es/oauth/authorize\n    tokenUrl: https://coupondroid.es/oauth/token\n    scopes: 3\n  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.\n  sources:\n  - openapi/coupondroid-es-openapi.yml\n  - https://coupondroid.es/auth.md\n  pkce: S256 only\n  dynamic_client_registration: https://coupondroid.es/oauth/register\n  refresh: grant_type=refresh_token\n  revocation_url: https://coupondroid.es/oauth/revoke\n  token_placement: 'Authorization: Bearer header'\n  discovery:\n  - https://coupondroid.es/.well-known/oauth-protected-resource\n  - https://coupondroid.es/.well-known/oauth-authorization-server\n  applies_to:\n  - managementMcp\ndocs: https://coupondroid.es/auth.md\n\
  unauthenticated:\n  operations:\n  - publicMcp\n  - a2aAgent\n  - health\n  - llmsTxt\n  - authMd\n  - mcpServerCard\n  - agentCard\n  - agentSkills\n  quote: 'Public agent APIs: no authentication.'\nnote: Management MCP tokens belong to a Coupondroid team member who signs in and approves the connection; agents\n  cannot self-register accounts.\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-es/authentication/coupondroid-es-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Shopping
- Spain
- MCP
---
