---
anonymous_access: false
api_key_in: []
api_specs:
- filename: realmarketapi-market-data-api-openapi.yml
  format: yaml
  label: RealMarketAPI Market Data API
  slug: realmarketapi-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realmarketapi/openapi/realmarketapi-market-data-api-openapi.yml
auth_types: []
description: RealMarketAPI uses an API key passed as a query parameter for both REST, WebSocket, and MCP endpoints.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Realmarketapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealMarketAPI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: RealMarketAPI
provider_slug: realmarketapi
scheme_count: 2
schemes:
- evidence: Authentication ?apiKey=YOUR_KEY
  how_to_obtain: Generate and manage your keys from the dashboard.
  location: query
  name: apiKey
  type: apiKey
- evidence: Pass an API key as a plain string argument named apiKey . Keys are obtained from the account dashboard .
  how_to_obtain: Keys are obtained from the account dashboard.
  location: query
  name: apiKey
  type: apiKey
slug: realmarketapi-authentication
source_filename: realmarketapi-authentication.yml
source_heading: Authentication Profile
source_url: https://realmarketapi.com/en-US/register
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://realmarketapi.com/en-US/register\nsources:\n- https://realmarketapi.com/en-US/register\n- https://realmarketapi.com/en-US/docs/getting-started\n- https://realmarketapi.com/en-US/docs/mcp\ndescription: RealMarketAPI uses an API key passed as a query parameter for both REST, WebSocket, and MCP endpoints.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Authentication ?apiKey=YOUR_KEY\n  location: query\n  how_to_obtain: Generate and manage your keys from the dashboard.\n- type: apiKey\n  name: apiKey\n  evidence: Pass an API key as a plain string argument named apiKey . Keys are obtained from the account dashboard .\n  location: query\n  how_to_obtain: Keys are obtained from the account dashboard.\ndocs: https://realmarketapi.com/en-US/register\n"
source_yaml_url: https://artifacts.apis.io/realmarketapi/authentication/realmarketapi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fintech
- Market Data
- Real-Time
---
