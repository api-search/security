---
anonymous_access: false
api_key_in: []
api_specs:
- filename: equibles-openapi-generated.yml
  format: yaml
  label: Equibles API
  slug: equibles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equibles/refs/heads/main/openapi/_ae-authored/equibles-openapi-generated.yml
auth_types: []
description: Authentication methods for Equibles
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Equibles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equibles declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Equibles
provider_slug: equibles
scheme_count: 2
schemes:
- evidence: The REST API uses an API key . MCP data requests accept an API key or, in supported clients, OAuth , so there's no key to copy or store.
  header: Authorization
  how_to_obtain: Create keys in your dashboard. A key starts with the prefix eq_ and is shown once at creation.
  location: header
  name: API key
  type: apiKey
- evidence: 'Query parameter — useful where you can''t set headers (for example an MCP client that only takes a URL): https://api.equibles.com/v1/stocks/AAPL/prices?api_key=eq_your_api_key'
  how_to_obtain: Create keys in your dashboard. A key starts with the prefix eq_ and is shown once at creation.
  location: query
  name: API key (query)
  type: apiKey
slug: equibles-authentication
source_filename: equibles-authentication.yml
source_heading: Authentication Profile
source_url: https://equibles.com/docs/authentication
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://equibles.com/docs/authentication\nsources:\n- https://equibles.com/docs/authentication\n- https://equibles.com/docs/mcp/claude-web\n- https://equibles.com/docs/mcp/claude-desktop\n- https://equibles.com/docs\ndescription: Authentication methods for Equibles\nschemes:\n- type: apiKey\n  name: API key\n  evidence: The REST API uses an API key . MCP data requests accept an API key or, in supported clients, OAuth , so there's no key to copy or\n    store.\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in your dashboard. A key starts with the prefix eq_ and is shown once at creation.\n- type: apiKey\n  name: API key (query)\n  evidence: 'Query parameter — useful where you can''t set headers (for example an MCP client that only takes a URL): https://api.equibles.com/v1/stocks/AAPL/prices?api_key=eq_your_api_key'\n  location: query\n  how_to_obtain:\
  \ Create keys in your dashboard. A key starts with the prefix eq_ and is shown once at creation.\ndocs: https://equibles.com/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equibles/refs/heads/main/authentication/equibles-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- API
- Stocks
---
