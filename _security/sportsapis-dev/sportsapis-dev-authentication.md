---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sportsapis-dev-openapi-generated.yml
  format: yaml
  label: SportsAPIs.dev API
  slug: sportsapis-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsapis-dev/refs/heads/main/openapi/_ae-authored/sportsapis-dev-openapi-generated.yml
auth_types: []
description: Authentication uses an API key passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sportsapis Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: SportsAPIs.dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SportsAPIs.dev
provider_slug: sportsapis-dev
scheme_count: 1
schemes:
- evidence: GET /sports/{sport}/odds ?apiKey={your_api_key}
  how_to_obtain: Generate your API key in the provider's dashboard after signing up.
  location: query
  name: API Key
  type: apiKey
slug: sportsapis-dev-authentication
source_filename: sportsapis-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://sportsapis.dev/sports-mcp-servers#sportsapis-mcp
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sportsapis.dev/sports-mcp-servers#sportsapis-mcp\nsources:\n- https://sportsapis.dev/sports-mcp-servers#sportsapis-mcp\n- https://sportsapis.dev/guides/getting-started\ndescription: Authentication uses an API key passed as a query parameter.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: GET /sports/{sport}/odds ?apiKey={your_api_key}\n  location: query\n  how_to_obtain: Generate your API key in the provider's dashboard after signing up.\nnote: No other authentication methods (OAuth, HTTP, etc.) are documented on the provided pages.\ndocs: https://sportsapis.dev/sports-mcp-servers#sportsapis-mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsapis-dev/refs/heads/main/authentication/sportsapis-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sports
- Odds
- Data
- Gambling
---
