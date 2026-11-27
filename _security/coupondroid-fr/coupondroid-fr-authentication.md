---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coupondroid-fr-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid France A2a API
  slug: coupondroid-fr-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-a2a-api-openapi.yml
- filename: coupondroid-fr-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid France Auth.md API
  slug: coupondroid-fr-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-auth-md-api-openapi.yml
- filename: coupondroid-fr-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid France Llms.txt API
  slug: coupondroid-fr-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-llms-txt-api-openapi.yml
- filename: coupondroid-fr-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid France MCP API
  slug: coupondroid-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-mcp-api-openapi.yml
- filename: coupondroid-fr-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid France .well Known API
  slug: coupondroid-fr-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid France Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid France secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid France
provider_slug: coupondroid-fr
scheme_count: 1
schemes:
- applies_to:
  - managementMcp
  audience: Coupondroid team members only; agents cannot create accounts
  authorization_server_metadata: https://coupondroid.fr/.well-known/oauth-authorization-server (RFC 8414, HTTP 200)
  bearer: 'Authorization: Bearer header'
  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  dynamic_client_registration: POST https://coupondroid.fr/oauth/register (RFC 7591); public clients use token_endpoint_auth_method none
  flows:
  - authorizationUrl: https://coupondroid.fr/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://coupondroid.fr/oauth/token
  name: oauth2
  pkce: S256 only
  protected_resource_metadata: https://coupondroid.fr/.well-known/oauth-protected-resource (RFC 9728, HTTP 200)
  refresh: grant_type=refresh_token
  revocation: https://coupondroid.fr/oauth/revoke
  sources:
  - openapi/coupondroid-fr-openapi.yml
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: coupondroid-fr-authentication
source_filename: coupondroid-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.fr/auth.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.fr/oauth/authorize\n    tokenUrl: https://coupondroid.fr/oauth/token\n    scopes: 3\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\n  sources:\n  - openapi/coupondroid-fr-openapi.yml\n  pkce: S256 only\n  dynamic_client_registration: POST https://coupondroid.fr/oauth/register (RFC 7591);\n    public clients use token_endpoint_auth_method none\n  bearer: 'Authorization: Bearer header'\n  refresh: grant_type=refresh_token\n  revocation: https://coupondroid.fr/oauth/revoke\n  protected_resource_metadata: https://coupondroid.fr/.well-known/oauth-protected-resource\n    (RFC 9728, HTTP 200)\n  authorization_server_metadata: https://coupondroid.fr/.well-known/oauth-authorization-server\n\
  \    (RFC 8414, HTTP 200)\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  applies_to:\n  - managementMcp\n  audience: Coupondroid team members only; agents cannot create accounts\ndocs: https://coupondroid.fr/auth.md\nderived_from: openapi/coupondroid-fr-openapi.yml\npublic_surface:\n  operations:\n  - publicMcp\n  - a2aAgent\n  - health\n  - llmsTxt\n  - authMd\n  - mcpServerCard\n  - agentCard\n  - agentSkills\n  auth: none\n  quote: 'Public agent APIs: no authentication.'\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-fr/authentication/coupondroid-fr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Coupons
- Promo Codes
- Deals
- E-Commerce
- Affiliate Marketing
- France
- MCP
---
