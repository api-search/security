---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marinergps-tools-openapi-generated.yml
  format: yaml
  label: Mariner GPS Tools API
  slug: marinergps-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marinergps-tools/openapi/_ae-authored/marinergps-tools-openapi-generated.yml
auth_types: []
description: Authentication methods for Mariner GPS Tools API and MCP.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mariner GPS Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mariner GPS Tools declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mariner GPS Tools
provider_slug: marinergps-tools
scheme_count: 2
schemes:
- evidence: Applications, services, scripts and manual integrations use a Mariner GPS Tools API key sent as a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key via the account page; keys are free to create and can be rotated or revoked at any time.
  location: header
  name: Authorization
  type: apiKey
- evidence: Interactive AI clients connect to the MCP server and authorize access in the browser with OAuth.
  name: OAuth
  type: oauth2
slug: marinergps-tools-authentication
source_filename: marinergps-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://marinergps.tools/api/docs/
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://marinergps.tools/api/docs/\nsources:\n- https://marinergps.tools/api/docs/\n- https://marinergps.tools/api/docs/mcp/\ndescription: Authentication methods for Mariner GPS Tools API and MCP.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Applications, services, scripts and manual integrations use a Mariner GPS Tools API key sent as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the account page; keys are free to create and can be rotated or revoked at any time.\n- type: oauth2\n  name: OAuth\n  evidence: Interactive AI clients connect to the MCP server and authorize access in the browser with OAuth.\ndocs: https://marinergps.tools/api/docs/\n"
source_yaml_url: https://artifacts.apis.io/marinergps-tools/authentication/marinergps-tools-authentication.yml
summary_line: 2 schemes
tags:
- Marine
- Navigation
- GPS
- Calculators
---
