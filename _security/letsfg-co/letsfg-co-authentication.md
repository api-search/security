---
anonymous_access: false
api_key_in: []
api_specs:
- filename: letsfg-co-agents-api-openapi.yml
  format: yaml
  label: LetsFG Agents API
  slug: letsfg-co-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-agents-api-openapi.yml
- filename: letsfg-co-flights-api-openapi.yml
  format: yaml
  label: LetsFG Flights API
  slug: letsfg-co-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-flights-api-openapi.yml
- filename: letsfg-co-hotels-api-openapi.yml
  format: yaml
  label: LetsFG Hotels API
  slug: letsfg-co-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-hotels-api-openapi.yml
- filename: letsfg-co-sandbox-api-openapi.yml
  format: yaml
  label: LetsFG Sandbox API
  slug: letsfg-co-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsfg-co/openapi/letsfg-co-sandbox-api-openapi.yml
auth_types: []
description: 'LetsFG supports two authentication schemes: a Bearer token obtained from the connect flow (used for free PFS searches and bookings) and an API key issued after registration (used for the Public Developer API).'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LetsFG Authentication
name_suffix: Authentication
oauth_flows: []
overview: LetsFG declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LetsFG
provider_slug: letsfg-co
scheme_count: 2
schemes:
- evidence: Programmatic access requires the token from the connect flow
  header: Authorization
  how_to_obtain: Connect LetsFG as an MCP server at https://letsfg.co/mcp and approve the connection; the consent step opens https://letsfg.co/connect and returns a token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Requests require an API key.
  header: X-API-Key
  how_to_obtain: Register via POST /agents/register to receive an api_key, then use that key in the X-API-Key header.
  location: header
  name: Developer API key
  type: apiKey
slug: letsfg-co-authentication
source_filename: letsfg-co-authentication.yml
source_heading: Authentication Profile
source_url: https://letsfg.co/developers/docs/agent-guide/index.html
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://letsfg.co/developers/docs/agent-guide/index.html\nsources:\n- https://letsfg.co/developers/docs/agent-guide/index.html\n- https://letsfg.co/developers/api/docs#/agents/post_agents_setup_payment\n- https://letsfg.co/developers/api/docs\n- https://letsfg.co/developers/docs/getting-started/index.html\ndescription: 'LetsFG supports two authentication schemes: a Bearer token obtained from the connect flow (used for free PFS searches and bookings)\n  and an API key issued after registration (used for the Public Developer API).'\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Programmatic access requires the token from the connect flow\n  location: header\n  header: Authorization\n  how_to_obtain: Connect LetsFG as an MCP server at https://letsfg.co/mcp and approve the connection; the consent step opens https://letsfg.co/connect\n    and returns a token.\n- type:\
  \ apiKey\n  name: Developer API key\n  evidence: Requests require an API key.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Register via POST /agents/register to receive an api_key, then use that key in the X-API-Key header.\ndocs: https://letsfg.co/developers/docs/agent-guide/index.html\n"
source_yaml_url: https://artifacts.apis.io/letsfg-co/authentication/letsfg-co-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- Artificial Intelligence
- Booking
- Flights
- Hotels
---
