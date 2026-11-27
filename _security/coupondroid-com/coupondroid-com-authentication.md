---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coupondroid-com-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid A2a API
  slug: coupondroid-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-a2a-api-openapi.yml
- filename: coupondroid-com-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Auth.md API
  slug: coupondroid-com-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-auth-md-api-openapi.yml
- filename: coupondroid-com-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Llms.txt API
  slug: coupondroid-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-llms-txt-api-openapi.yml
- filename: coupondroid-com-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid MCP API
  slug: coupondroid-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-mcp-api-openapi.yml
- filename: coupondroid-com-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid .well Known API
  slug: coupondroid-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-well-known-api-openapi.yml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupondroid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coupondroid secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coupondroid
provider_slug: coupondroid-com
scheme_count: 2
schemes:
- applies_to:
  - https://coupondroid.com/mcp/public
  - https://coupondroid.com/a2a
  description: 'Public agent APIs: no authentication. Read-only and open to any agent; there is nothing to register.'
  name: none
  type: none
- applies_to:
  - https://coupondroid.com/mcp
  description: Team only. Every token belongs to a Coupondroid team member who signed in (password and optional 2FA) and approved the connection; agents cannot create accounts. Effective permission is the smaller of the token scopes and the person's role. Connections are visible/revocable at https://coupondroid.com/oauth/connections.
  discovery:
  - https://coupondroid.com/.well-known/oauth-protected-resource (RFC 9728)
  - https://coupondroid.com/.well-known/oauth-authorization-server (RFC 8414)
  dynamic_client_registration: RFC 7591; public clients use token_endpoint_auth_method none; registering a client does not give access by itself.
  flows:
  - authorizationUrl: https://coupondroid.com/oauth/authorize
    flow: authorizationCode
    pkce: S256 only
    refreshUrl: https://coupondroid.com/oauth/token
    registrationUrl: https://coupondroid.com/oauth/register
    revocationUrl: https://coupondroid.com/oauth/revoke
    scopes: 3
    tokenUrl: https://coupondroid.com/oauth/token
  name: oauth2
  sources:
  - openapi/coupondroid-com-openapi.yml
  - https://coupondroid.com/auth.md
  token_placement: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: coupondroid-com-authentication
source_filename: coupondroid-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.com/auth.md\ndocs: https://coupondroid.com/auth.md\nsummary:\n  types:\n  - none\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  note: Public MCP server (/mcp/public) and A2A agent (/a2a) require no authentication; only the team-only management MCP server (/mcp) uses OAuth 2.1.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://coupondroid.com/mcp/public\n  - https://coupondroid.com/a2a\n  description: 'Public agent APIs: no authentication. Read-only and open to any agent; there is nothing to register.'\n- name: oauth2\n  type: oauth2\n  applies_to:\n  - https://coupondroid.com/mcp\n  flows:\n  - flow: authorizationCode\n    pkce: S256 only\n    authorizationUrl: https://coupondroid.com/oauth/authorize\n    tokenUrl: https://coupondroid.com/oauth/token\n    refreshUrl: https://coupondroid.com/oauth/token\n    revocationUrl: https://coupondroid.com/oauth/revoke\n    registrationUrl:\
  \ https://coupondroid.com/oauth/register\n    scopes: 3\n  token_placement: 'Authorization: Bearer <access_token>'\n  discovery:\n  - https://coupondroid.com/.well-known/oauth-protected-resource (RFC 9728)\n  - https://coupondroid.com/.well-known/oauth-authorization-server (RFC 8414)\n  dynamic_client_registration: RFC 7591; public clients use token_endpoint_auth_method none; registering a client does not give access by itself.\n  description: Team only. Every token belongs to a Coupondroid team member who signed in (password and optional 2FA) and approved the connection; agents cannot create accounts. Effective permission is the smaller of the token scopes and the person's role. Connections are visible/revocable at https://coupondroid.com/oauth/connections.\n  sources:\n  - openapi/coupondroid-com-openapi.yml\n  - https://coupondroid.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-com/authentication/coupondroid-com-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Coupons
- Deals
- E-Commerce
- Shopping
- Affiliate Marketing
- MCP
- AI Agents
---
