---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coupondroid-mx-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid México A2a API
  slug: coupondroid-mx-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-a2a-api-openapi.yml
- filename: coupondroid-mx-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid México Auth.md API
  slug: coupondroid-mx-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-auth-md-api-openapi.yml
- filename: coupondroid-mx-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid México Llms.txt API
  slug: coupondroid-mx-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-llms-txt-api-openapi.yml
- filename: coupondroid-mx-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid México MCP API
  slug: coupondroid-mx-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-mcp-api-openapi.yml
- filename: coupondroid-mx-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid México .well Known API
  slug: coupondroid-mx-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-well-known-api-openapi.yml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid México Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid México secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid México
provider_slug: coupondroid-mx
scheme_count: 2
schemes:
- applies_to:
  - publicMcp
  - a2aAgent
  description: 'Public agent APIs: no authentication. Limit: 120 requests per minute per IP.'
  name: none
  sources:
  - https://coupondroid.mx/auth.md
  type: none
- applies_to:
  - managementMcp
  description: Authorization code with PKCE (S256); dynamic client registration (RFC 7591) at /oauth/register, public clients use token_endpoint_auth_method none. Every token belongs to a team member who signed in and approved the connection; agents cannot create accounts. Effective permission is the smaller of the token scopes and the person's role.
  discovery:
  - https://coupondroid.mx/.well-known/oauth-protected-resource
  - https://coupondroid.mx/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://coupondroid.mx/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://coupondroid.mx/oauth/token
    registrationUrl: https://coupondroid.mx/oauth/register
    revocationUrl: https://coupondroid.mx/oauth/revoke
    scopes: 3
    tokenUrl: https://coupondroid.mx/oauth/token
  name: oauth2
  sources:
  - openapi/coupondroid-mx-openapi.yml
  - https://coupondroid.mx/auth.md
  token_placement: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: coupondroid-mx-authentication
source_filename: coupondroid-mx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.mx/auth.md\ndocs: https://coupondroid.mx/auth.md\nsummary:\n  types:\n  - none\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  note: Public MCP (/mcp/public) and A2A (/a2a) are read-only and need no authentication (\"There is nothing to register\").\n    Only the management MCP server (/mcp) uses OAuth 2.1, and only for members of the Coupondroid México team.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - publicMcp\n  - a2aAgent\n  description: 'Public agent APIs: no authentication. Limit: 120 requests per minute per IP.'\n  sources:\n  - https://coupondroid.mx/auth.md\n- name: oauth2\n  type: oauth2\n  applies_to:\n  - managementMcp\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://coupondroid.mx/oauth/authorize\n    tokenUrl: https://coupondroid.mx/oauth/token\n    refreshUrl: https://coupondroid.mx/oauth/token\n    revocationUrl: https://coupondroid.mx/oauth/revoke\n\
  \    registrationUrl: https://coupondroid.mx/oauth/register\n    scopes: 3\n  token_placement: 'Authorization: Bearer <access_token>'\n  discovery:\n  - https://coupondroid.mx/.well-known/oauth-protected-resource\n  - https://coupondroid.mx/.well-known/oauth-authorization-server\n  description: Authorization code with PKCE (S256); dynamic client registration (RFC 7591) at /oauth/register, public\n    clients use token_endpoint_auth_method none. Every token belongs to a team member who signed in and approved the\n    connection; agents cannot create accounts. Effective permission is the smaller of the token scopes and the person's role.\n  sources:\n  - openapi/coupondroid-mx-openapi.yml\n  - https://coupondroid.mx/auth.md\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-mx/authentication/coupondroid-mx-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Coupons
- Discounts
- Deals
- E-Commerce
- Mexico
- Affiliate Marketing
- MCP
---
