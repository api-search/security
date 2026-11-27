---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadstrategist-dk-account-api-openapi.yml
  format: yaml
  label: Lead Strategist Account API
  slug: leadstrategist-dk-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-account-api-openapi.yml
- filename: leadstrategist-dk-companies-api-openapi.yml
  format: yaml
  label: Lead Strategist Companies API
  slug: leadstrategist-dk-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-companies-api-openapi.yml
- filename: leadstrategist-dk-meta-api-openapi.yml
  format: yaml
  label: Lead Strategist Meta API
  slug: leadstrategist-dk-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-meta-api-openapi.yml
auth_types: []
description: Authentication methods for Lead Strategist MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lead Strategist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Strategist declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lead Strategist
provider_slug: leadstrategist-dk
scheme_count: 2
schemes:
- evidence: 'Send Authorization: Bearer ls_live_… (or x-api-key: ls_live_… ) with every request.'
  header: Authorization
  location: header
  name: API key
  type: http-bearer
- authorize_url: https://leadstrategist.dk/authorize
  evidence: Sign in with your Lead Strategist account and click Allow connection.
  how_to_obtain: 'Public clients only ( token_endpoint_auth_method: none ) with PKCE S256. Register dynamically at https://leadstrategist.dk/register and use the authorization endpoint with PKCE to obtain an authorization code, then exchange it for an access token at the token endpoint.'
  name: OAuth 2.1 with PKCE
  scopes:
  - cvr:read
  - offline_access
  token_url: https://leadstrategist.dk/token
  type: oauth2
slug: leadstrategist-dk-authentication
source_filename: leadstrategist-dk-authentication.yml
source_heading: Authentication Profile
source_url: https://leadstrategist.dk/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://leadstrategist.dk/.well-known/oauth-protected-resource/mcp\nsources:\n- https://leadstrategist.dk/.well-known/oauth-protected-resource/mcp\n- https://leadstrategist.dk/.well-known/oauth-authorization-server\n- https://leadstrategist.dk/docs/mcp\n- https://leadstrategist.dk/en/docs/mcp\ndescription: Authentication methods for Lead Strategist MCP\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send Authorization: Bearer ls_live_… (or x-api-key: ls_live_… ) with every request.'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Sign in with your Lead Strategist account and click Allow connection.\n  token_url: https://leadstrategist.dk/token\n  authorize_url: https://leadstrategist.dk/authorize\n  scopes:\n  - cvr:read\n  - offline_access\n  how_to_obtain: 'Public clients only ( token_endpoint_auth_method: none\
  \ ) with PKCE S256. Register dynamically at https://leadstrategist.dk/register\n    and use the authorization endpoint with PKCE to obtain an authorization code, then exchange it for an access token at the token endpoint.'\ndocs: https://leadstrategist.dk/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/leadstrategist-dk/authentication/leadstrategist-dk-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Data
- Finance
- Denmark
- CVR
---
