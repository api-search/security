---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gummble-com-api-openapi-generated.yml
  format: yaml
  label: Gummble API Reference API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-api-openapi-generated.yml
- filename: gummble-com-core-openapi-generated.yml
  format: yaml
  label: Gummble core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-core-openapi-generated.yml
- filename: gummble-com-mcp-openapi-generated.yml
  format: yaml
  label: Gummble MCP API
  slug: mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-mcp-openapi-generated.yml
auth_types: []
description: Authentication schemes published for Gummble
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gummble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gummble declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gummble
provider_slug: gummble-com
scheme_count: 1
schemes:
- authorize_url: https://api.gummble.com/oauth/authorize
  evidence: Gummble runs a standards-compliant OAuth 2.1 Authorization Server at https://api.gummble.com.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register a client via POST https://api.gummble.com/oauth/register, then perform the PKCE authorization code flow to receive an access token.
  name: OAuth 2.1
  scopes:
  - mcp:read
  - mcp:tools
  type: oauth2
slug: gummble-com-authentication
source_filename: gummble-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.gummble.com/docs/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.gummble.com/docs/authentication\nsources:\n- https://docs.gummble.com/docs/authentication\n- https://docs.gummble.com/docs/mcp/oauth\n- https://docs.gummble.com/docs/mcp/cursor\n- https://docs.gummble.com/docs/mcp/bolt\ndescription: Authentication schemes published for Gummble\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Gummble runs a standards-compliant OAuth 2.1 Authorization Server at https://api.gummble.com.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://api.gummble.com/oauth/authorize\n  scopes:\n  - mcp:read\n  - mcp:tools\n  how_to_obtain: Register a client via POST https://api.gummble.com/oauth/register, then perform the PKCE authorization code flow to receive an\n    access token.\ndocs: https://docs.gummble.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/gummble-com/authentication/gummble-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- UI
- Design
- Screenshots
---
