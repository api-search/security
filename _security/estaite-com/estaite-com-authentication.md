---
anonymous_access: false
api_key_in: []
api_specs:
- filename: estaite-com-openapi-generated.yml
  format: yaml
  label: Estaite Solutions API
  slug: estaite-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/estaite-com/openapi/_ae-authored/estaite-com-openapi-generated.yml
auth_types: []
description: Authentication options for Estaite MCP as published on the documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Estaite Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Estaite Solutions declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Estaite Solutions
provider_slug: estaite-com
scheme_count: 3
schemes:
- evidence: Option 1 — x-api-key header (preferred) Recommended for any code‑driven client ( mcp-remote , custom agents, curl , HTTP libraries).
  header: x-api-key
  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Option 2 — Authorization: Bearer For clients that complete the OAuth 2.1 authorization‑code flow (e.g. Claude.ai web’s custom‑connector flow), the resulting access token is your API key, and it’s sent as a Bearer token.'
  header: Authorization
  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Option 3 — ?key= query string The standard auth method for clients that only accept a URL and don’t expose request headers — Claude Desktop Connectors , ChatGPT custom GPTs, embedded integrations, and anywhere you need a single shareable URL configuration.
  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.
  location: query
  name: key
  type: apiKey
slug: estaite-com-authentication
source_filename: estaite-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.estaite.com/authentication/
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.estaite.com/authentication/\nsources:\n- https://docs.estaite.com/authentication/\n- https://docs.estaite.com/quickstart/\n- https://docs.estaite.com/quickstart/\ndescription: Authentication options for Estaite MCP as published on the documentation pages.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Option 1 — x-api-key header (preferred) Recommended for any code‑driven client ( mcp-remote , custom agents, curl , HTTP libraries).\n  location: header\n  header: x-api-key\n  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Option 2 — Authorization: Bearer For clients that complete the OAuth 2.1 authorization‑code flow (e.g. Claude.ai web’s custom‑connector\n    flow), the resulting access token is your API key, and it’s sent as a Bearer token.'\n  location: header\n  header:\
  \ Authorization\n  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.\n- type: apiKey\n  name: key\n  evidence: Option 3 — ?key= query string The standard auth method for clients that only accept a URL and don’t expose request headers — Claude\n    Desktop Connectors , ChatGPT custom GPTs, embedded integrations, and anywhere you need a single shareable URL configuration.\n  location: query\n  how_to_obtain: API keys are issued from the estaite.com/developers dashboard.\ndocs: https://docs.estaite.com/authentication/\n"
source_yaml_url: https://artifacts.apis.io/estaite-com/authentication/estaite-com-authentication.yml
summary_line: 3 schemes
tags:
- Real Estate
- Lead Generation
- Data Analytics
- Property Management
- Software-as-a-Service
- Company
---
