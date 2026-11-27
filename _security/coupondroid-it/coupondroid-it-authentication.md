---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coupondroid-it-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Italia A2a API
  slug: coupondroid-it-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-a2a-api-openapi.yml
- filename: coupondroid-it-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Italia Auth.md API
  slug: coupondroid-it-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-auth-md-api-openapi.yml
- filename: coupondroid-it-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Italia Llms.txt API
  slug: coupondroid-it-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-llms-txt-api-openapi.yml
- filename: coupondroid-it-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Italia MCP API
  slug: coupondroid-it-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-mcp-api-openapi.yml
- filename: coupondroid-it-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Italia .well Known API
  slug: coupondroid-it-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid Italia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid Italia secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid Italia
provider_slug: coupondroid-it
scheme_count: 1
schemes:
- applies_to: Management MCP server https://coupondroid.it/mcp only (team members); tokens belong to a team member who signed in and approved the connection
  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  discovery:
  - https://coupondroid.it/.well-known/oauth-protected-resource (RFC 9728)
  - https://coupondroid.it/.well-known/oauth-authorization-server (RFC 8414)
  dynamic_client_registration: POST https://coupondroid.it/oauth/register (RFC 7591); public clients use token_endpoint_auth_method none
  flows:
  - authorizationUrl: https://coupondroid.it/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://coupondroid.it/oauth/token
  name: oauth2
  note: Documented in auth.md; not exercised by this pipeline (no auth endpoints were called).
  pkce: S256 only
  refreshUrl: https://coupondroid.it/oauth/token
  revocation_url: https://coupondroid.it/oauth/revoke
  sources:
  - openapi/coupondroid-it-openapi.yml
  token_location: 'Authorization: Bearer header'
  type: oauth2
slug: coupondroid-it-authentication
source_filename: coupondroid-it-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.it/auth.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  public_access: none required for /mcp/public and /a2a\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.it/oauth/authorize\n    tokenUrl: https://coupondroid.it/oauth/token\n    scopes: 3\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\n  sources:\n  - openapi/coupondroid-it-openapi.yml\n  pkce: S256 only\n  token_location: 'Authorization: Bearer header'\n  refreshUrl: https://coupondroid.it/oauth/token\n  revocation_url: https://coupondroid.it/oauth/revoke\n  dynamic_client_registration: POST https://coupondroid.it/oauth/register (RFC 7591);\n    public clients use token_endpoint_auth_method none\n  discovery:\n  - https://coupondroid.it/.well-known/oauth-protected-resource (RFC 9728)\n  -\
  \ https://coupondroid.it/.well-known/oauth-authorization-server (RFC 8414)\n  applies_to: Management MCP server https://coupondroid.it/mcp only (team members);\n    tokens belong to a team member who signed in and approved the connection\n  note: Documented in auth.md; not exercised by this pipeline (no auth endpoints were\n    called).\ndocs: https://coupondroid.it/auth.md\nunauthenticated:\n- endpoint: https://coupondroid.it/mcp/public\n  note: 'Public agent APIs: no authentication.'\n- endpoint: https://coupondroid.it/a2a\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-it/authentication/coupondroid-it-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Coupons
- Discount Codes
- Deals
- E-Commerce
- Affiliate Marketing
- Italy
- MCP
---
