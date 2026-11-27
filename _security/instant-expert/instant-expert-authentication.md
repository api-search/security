---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instant-expert-asks-api-openapi.yml
  format: yaml
  label: Instant Expert Asks API
  slug: instant-expert-asks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instant-expert/openapi/instant-expert-asks-api-openapi.yml
- filename: instant-expert-test-mode-api-openapi.yml
  format: yaml
  label: Instant Expert Test mode API
  slug: instant-expert-test-mode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instant-expert/openapi/instant-expert-test-mode-api-openapi.yml
auth_types: []
description: Authentication for the Instant Expert MCP server
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Instant Expert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instant Expert declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Instant Expert
provider_slug: instant-expert
scheme_count: 1
schemes:
- evidence: 'Auth: OAuth 2.1 authorization code flow with PKCE.'
  flows:
  - authorization_code
  how_to_obtain: Sign in via the browser when prompted; the server uses the OAuth 2.1 authorization code flow with PKCE and returns a bearer token to be sent in the Authorization header.
  name: OAuth 2.1
  scopes:
  - email
  - profile
  - offline_access
  type: oauth2
slug: instant-expert-authentication
source_filename: instant-expert-authentication.yml
source_heading: Authentication Profile
source_url: https://instant.expert/docs/mcp
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://instant.expert/docs/mcp\nsources:\n- https://instant.expert/docs/mcp\ndescription: Authentication for the Instant Expert MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Auth: OAuth 2.1 authorization code flow with PKCE.'\n  flows:\n  - authorization_code\n  scopes:\n  - email\n  - profile\n  - offline_access\n  how_to_obtain: Sign in via the browser when prompted; the server uses the OAuth 2.1 authorization code flow with PKCE and returns a bearer token\n    to be sent in the Authorization header.\ndocs: https://instant.expert/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/instant-expert/authentication/instant-expert-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Outreach
- Sales
- Artificial Intelligence
- MCP
- B2B
---
