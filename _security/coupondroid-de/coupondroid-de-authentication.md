---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coupondroid-de-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland A2a API
  slug: coupondroid-de-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-a2a-api-openapi.yml
- filename: coupondroid-de-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland Auth.md API
  slug: coupondroid-de-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-auth-md-api-openapi.yml
- filename: coupondroid-de-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland Llms.txt API
  slug: coupondroid-de-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-llms-txt-api-openapi.yml
- filename: coupondroid-de-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland MCP API
  slug: coupondroid-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-mcp-api-openapi.yml
- filename: coupondroid-de-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland .well Known API
  slug: coupondroid-de-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-well-known-api-openapi.yml
auth_types:
- none
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Coupondroid Deutschland Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid Deutschland secures its APIs with none, oauth2, and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid Deutschland
provider_slug: coupondroid-de
scheme_count: 3
schemes:
- applies_to:
  - https://coupondroid.de/mcp/public
  - https://coupondroid.de/a2a
  description: '"Public agent APIs: no authentication." Read-only, open to any agent, nothing to register (auth.md).'
  name: public
  type: none
- applies_to:
  - https://coupondroid.de/mcp
  authorization_server_metadata: https://coupondroid.de/.well-known/oauth-authorization-server (RFC 8414)
  description: Authorization code with PKCE on behalf of a team member. Agents cannot create accounts; every token belongs to a team member who signed in and approved the connection. Effective rights are the smaller of the token scopes and the person's role.
  dynamic_client_registration: https://coupondroid.de/oauth/register (RFC 7591; public clients use token_endpoint_auth_method none)
  flows:
  - authorizationUrl: https://coupondroid.de/oauth/authorize
    flow: authorizationCode
    pkce: S256 only
    refreshUrl: https://coupondroid.de/oauth/token
    scopes: 3
    tokenUrl: https://coupondroid.de/oauth/token
  name: oauth2
  protected_resource_metadata: https://coupondroid.de/.well-known/oauth-protected-resource (RFC 9728)
  revocation: https://coupondroid.de/oauth/revoke
  sources:
  - openapi/coupondroid-de-openapi.yml
  - https://coupondroid.de/auth.md
  token_placement: Authorization Bearer header
  type: oauth2
- applies_to:
  - https://coupondroid.de/mcp
  description: 'The OAuth about page states the management server also accepts "an ohmy_… token in the Authorization: Bearer header". Not declared in the OpenAPI.'
  name: ohmy-token
  scheme: bearer
  sources:
  - https://coupondroid.de/oauth/about
  type: http
slug: coupondroid-de-authentication
source_filename: coupondroid-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.de/auth.md\ndocs: https://coupondroid.de/auth.md\nsummary:\n  types:\n  - none\n  - oauth2\n  - http-bearer\n  oauth2_flows:\n  - authorizationCode\n  note: Public MCP server (/mcp/public), A2A agent (/a2a) and discovery documents need no authentication. Only the team management MCP server (/mcp) is protected.\nschemes:\n- name: public\n  type: none\n  applies_to:\n  - https://coupondroid.de/mcp/public\n  - https://coupondroid.de/a2a\n  description: '\"Public agent APIs: no authentication.\" Read-only, open to any agent, nothing to register (auth.md).'\n- name: oauth2\n  type: oauth2\n  applies_to:\n  - https://coupondroid.de/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.de/oauth/authorize\n    tokenUrl: https://coupondroid.de/oauth/token\n    refreshUrl: https://coupondroid.de/oauth/token\n    pkce: S256 only\n    scopes: 3\n  dynamic_client_registration: https://coupondroid.de/oauth/register\
  \ (RFC 7591; public clients use token_endpoint_auth_method none)\n  revocation: https://coupondroid.de/oauth/revoke\n  protected_resource_metadata: https://coupondroid.de/.well-known/oauth-protected-resource (RFC 9728)\n  authorization_server_metadata: https://coupondroid.de/.well-known/oauth-authorization-server (RFC 8414)\n  token_placement: Authorization Bearer header\n  description: Authorization code with PKCE on behalf of a team member. Agents cannot create accounts; every token belongs to a team member who signed in and approved the connection. Effective rights are the smaller of the token scopes and the person's role.\n  sources:\n  - openapi/coupondroid-de-openapi.yml\n  - https://coupondroid.de/auth.md\n- name: ohmy-token\n  type: http\n  scheme: bearer\n  applies_to:\n  - https://coupondroid.de/mcp\n  description: 'The OAuth about page states the management server also accepts \"an ohmy_… token in the Authorization: Bearer header\". Not declared in the OpenAPI.'\n  sources:\n\
  \  - https://coupondroid.de/oauth/about\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-de/authentication/coupondroid-de-authentication.yml
summary_line: none/oauth2/http-bearer · 3 schemes
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Germany
- Shopping
- Vouchers
---
