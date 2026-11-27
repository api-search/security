---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flarewatch-io-openapi-generated.yml
  format: yaml
  label: FlareWatch API
  slug: flarewatch-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flarewatch-io/openapi/_ae-authored/flarewatch-io-openapi-generated.yml
auth_types: []
description: OAuth 2.0 authentication as defined by FlareWatch
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FlareWatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlareWatch declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FlareWatch
provider_slug: flarewatch-io
scheme_count: 1
schemes:
- authorize_url: https://www.flarewatch.io/api/mcp/oauth/authorize
  evidence: '"grant_types_supported":["authorization_code","refresh_token"]'
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register the client at https://www.flarewatch.io/api/mcp/oauth/register
  name: OAuth 2.0
  scopes:
  - public
  - wallet:read
  - personal:read
  type: oauth2
slug: flarewatch-io-authentication
source_filename: flarewatch-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.flarewatch.io/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.flarewatch.io/.well-known/oauth-authorization-server\nsources:\n- https://www.flarewatch.io/.well-known/oauth-authorization-server\n- https://www.flarewatch.io/.well-known/oauth-protected-resource\n- https://www.flarewatch.io/en/changelog#entry-2026-10-18-a\ndescription: OAuth 2.0 authentication as defined by FlareWatch\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: '\"grant_types_supported\":[\"authorization_code\",\"refresh_token\"]'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://www.flarewatch.io/api/mcp/oauth/authorize\n  scopes:\n  - public\n  - wallet:read\n  - personal:read\n  how_to_obtain: Register the client at https://www.flarewatch.io/api/mcp/oauth/register\ndocs: https://www.flarewatch.io/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/flarewatch-io/authentication/flarewatch-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Staking
- Dashboards
- Validator
- Tax
- DeFi
---
