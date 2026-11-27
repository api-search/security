---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CommercialBuses Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommercialBuses declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CommercialBuses
provider_slug: commercialbuses-com
scheme_count: 1
schemes:
- applies_to: https://commercialbuses.com/api/mcp
  description: Public MCP server; no credentials required.
  discovery_evidence: 'mcp.json servers[0].auth: "none"'
  evidence: CommercialBuses runs a public MCP server at https://commercialbuses.com/api/mcp (JSON-RPC 2.0 over HTTP POST, no account, no API key).
  type: none
slug: commercialbuses-com-authentication
source_filename: commercialbuses-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://commercialbuses.com/llms.txt\n- https://commercialbuses.com/.well-known/mcp.json\ndocs: https://commercialbuses.com/llms.txt\nschemes:\n- type: none\n  applies_to: https://commercialbuses.com/api/mcp\n  description: Public MCP server; no credentials required.\n  evidence: \"CommercialBuses runs a public MCP server at https://commercialbuses.com/api/mcp (JSON-RPC 2.0 over HTTP POST, no account, no API key).\"\n  discovery_evidence: 'mcp.json servers[0].auth: \"none\"'\nsummary: Unauthenticated. The only programmatic surface is the public MCP server, which the provider documents as needing no account and no API key. No OpenAPI and no OAuth exist.\n"
source_yaml_url: https://artifacts.apis.io/commercialbuses-com/authentication/commercialbuses-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Commercial Buses
- Vehicle Marketplace
- Transportation
- Dealers
- School Buses
- MCP
---
