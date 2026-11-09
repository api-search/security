---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airportloungelist-com-access-api-openapi.yml
  format: yaml
  label: Airport Lounge List Access API
  slug: airportloungelist-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-access-api-openapi.yml
- filename: airportloungelist-com-airports-api-openapi.yml
  format: yaml
  label: Airport Lounge List Airports API
  slug: airportloungelist-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-airports-api-openapi.yml
- filename: airportloungelist-com-lounges-api-openapi.yml
  format: yaml
  label: Airport Lounge List Lounges API
  slug: airportloungelist-com-lounges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-lounges-api-openapi.yml
- filename: airportloungelist-com-networks-api-openapi.yml
  format: yaml
  label: Airport Lounge List Networks API
  slug: airportloungelist-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-networks-api-openapi.yml
auth_types: []
description: OAuth 2.1 bearer token authentication for MCP tools
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Airportloungelist Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airport Lounge List declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Airport Lounge List
provider_slug: airportloungelist-com
scheme_count: 1
schemes:
- authorize_url: https://airportloungelist.com/oauth/authorize
  evidence: OAuth is required for all MCP tools, including the lounge-data tools. Follow the steps below before you call the MCP server.
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Dynamic Client Registration (RFC 7591) at https://mcp.airportloungelist.com/oauth/register returns a client_id; then use PKCE to obtain an authorization code and exchange it at the token endpoint for an access token.
  location: header
  name: Bearer
  scopes:
  - read
  - write
  type: http-bearer
slug: airportloungelist-com-authentication
source_filename: airportloungelist-com-authentication.yml
source_heading: Authentication Profile
source_url: https://airportloungelist.com/auth.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://airportloungelist.com/auth.md\nsources:\n- https://airportloungelist.com/auth.md\n- https://airportloungelist.com/setup.md\ndescription: OAuth 2.1 bearer token authentication for MCP tools\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: OAuth is required for all MCP tools, including the lounge-data tools. Follow the steps below before you call the MCP server.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://airportloungelist.com/oauth/authorize\n  scopes:\n  - read\n  - write\n  how_to_obtain: Dynamic Client Registration (RFC 7591) at https://mcp.airportloungelist.com/oauth/register returns a client_id; then use PKCE\n    to obtain an authorization code and exchange it at the token endpoint for an access token.\nnote: No API key or other authentication schemes are provided for the MCP\
  \ endpoint.\ndocs: https://airportloungelist.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/airportloungelist-com/authentication/airportloungelist-com-authentication.yml
summary_line: 1 scheme
tags:
- Airport
- Travel
- Lounge
- Aviation
- Comparison
- Company
---
