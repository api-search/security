---
anonymous_access: false
api_key_in: []
api_specs:
- filename: truckerfetch-v1-openapi.json
  format: json
  label: TruckerFetch Pro API V1 API
  slug: truckerfetch-pro-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truckerfetch/openapi/_original/truckerfetch-v1-openapi.json
auth_types: []
description: TruckerFetch authenticates REST requests with a scoped API key passed as a Bearer token in the Authorization header, and authenticates hosted MCP requests with an OAuth flow.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: TruckerFetch Authentication
name_suffix: Authentication
oauth_flows: []
overview: TruckerFetch declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TruckerFetch
provider_slug: truckerfetch
scheme_count: 2
schemes:
- evidence: 'Pass your secret over HTTPS in the bearer header: Authorization : Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create, rotate and revoke purpose‑specific keys in the API keys dashboard.
  location: header
  name: REST API key
  type: http-bearer
- evidence: Add https://truckerfetch.com/api/mcp to a compatible remote MCP client and follow its OAuth sign‑in flow.
  how_to_obtain: Use the hosted MCP client to initiate the OAuth sign‑in flow; an API key is not a hosted MCP OAuth token.
  name: Hosted MCP OAuth
  type: oauth2
slug: truckerfetch-authentication
source_filename: truckerfetch-authentication.yml
source_heading: Authentication Profile
source_url: https://truckerfetch.com/docs/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://truckerfetch.com/docs/authentication\nsources:\n- https://truckerfetch.com/docs/authentication\n- https://truckerfetch.com/docs/quickstart\ndescription: TruckerFetch authenticates REST requests with a scoped API key passed as a Bearer token in the Authorization header, and authenticates\n  hosted MCP requests with an OAuth flow.\nschemes:\n- type: http-bearer\n  name: REST API key\n  evidence: 'Pass your secret over HTTPS in the bearer header: Authorization : Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create, rotate and revoke purpose‑specific keys in the API keys dashboard.\n- type: oauth2\n  name: Hosted MCP OAuth\n  evidence: Add https://truckerfetch.com/api/mcp to a compatible remote MCP client and follow its OAuth sign‑in flow.\n  how_to_obtain: Use the hosted MCP client to initiate the OAuth sign‑in flow; an API key is not a\
  \ hosted MCP OAuth token.\ndocs: https://truckerfetch.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/truckerfetch/authentication/truckerfetch-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DOT
- Carrier
- Leads
- Transportation
---
