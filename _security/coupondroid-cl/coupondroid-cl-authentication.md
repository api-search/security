---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coupondroid-cl-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Chile A2a API
  slug: coupondroid-cl-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-a2a-api-openapi.yml
- filename: coupondroid-cl-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Auth.md API
  slug: coupondroid-cl-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-auth-md-api-openapi.yml
- filename: coupondroid-cl-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Llms.txt API
  slug: coupondroid-cl-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-llms-txt-api-openapi.yml
- filename: coupondroid-cl-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Chile MCP API
  slug: coupondroid-cl-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-mcp-api-openapi.yml
- filename: coupondroid-cl-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Chile .well Known API
  slug: coupondroid-cl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid Chile Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid Chile secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid Chile
provider_slug: coupondroid-cl
scheme_count: 1
schemes:
- applies_to:
  - managementMcp
  authorization_server_metadata: https://coupondroid.cl/.well-known/oauth-authorization-server (RFC 8414)
  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  dynamic_client_registration: https://coupondroid.cl/oauth/register (RFC 7591)
  flows:
  - authorizationUrl: https://coupondroid.cl/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://coupondroid.cl/oauth/token
  name: oauth2
  note: Per auth.md, tokens are issued only on behalf of a Coupondroid Chile team member who signs in and approves the connection; agents cannot create accounts. Effective rights are the smaller of the token scopes and the person's role.
  pkce: S256 only
  protected_resource_metadata: https://coupondroid.cl/.well-known/oauth-protected-resource (RFC 9728)
  refreshUrl: https://coupondroid.cl/oauth/token
  revocation_endpoint: https://coupondroid.cl/oauth/revoke
  sources:
  - openapi/coupondroid-cl-openapi.yml
  token_placement: 'Authorization: Bearer header'
  type: oauth2
slug: coupondroid-cl-authentication
source_filename: coupondroid-cl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.cl/auth.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  public_unauthenticated:\n  - publicMcp\n  - a2aAgent\n  - health\n  - llmsTxt\n  - authMd\n  - mcpServerCard\n  - agentCard\n  - agentSkills\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.cl/oauth/authorize\n    tokenUrl: https://coupondroid.cl/oauth/token\n    scopes: 3\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\n  sources:\n  - openapi/coupondroid-cl-openapi.yml\n  pkce: S256 only\n  token_placement: 'Authorization: Bearer header'\n  refreshUrl: https://coupondroid.cl/oauth/token\n  revocation_endpoint: https://coupondroid.cl/oauth/revoke\n  dynamic_client_registration: https://coupondroid.cl/oauth/register (RFC 7591)\n  protected_resource_metadata: https://coupondroid.cl/.well-known/oauth-protected-resource\n\
  \    (RFC 9728)\n  authorization_server_metadata: https://coupondroid.cl/.well-known/oauth-authorization-server\n    (RFC 8414)\n  applies_to:\n  - managementMcp\n  note: Per auth.md, tokens are issued only on behalf of a Coupondroid Chile team\n    member who signs in and approves the connection; agents cannot create accounts.\n    Effective rights are the smaller of the token scopes and the person's role.\ndocs: https://coupondroid.cl/auth.md\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-cl/authentication/coupondroid-cl-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Affiliate Marketing
- Retail
- Chile
- MCP
---
