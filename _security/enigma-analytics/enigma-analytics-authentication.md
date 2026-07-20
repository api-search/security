---
api_key_in:
- header
auth_types:
- apiKey
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Enigma Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enigma Analytics secures its APIs with apiKey and bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enigma Analytics
provider_slug: enigma-analytics
scheme_count: 2
schemes:
- applies_to: Enigma GraphQL API (https://api.enigma.com/graphql)
  description: All GraphQL API requests require an x-api-key request header carrying an Enigma API key issued from the Enigma Console (https://console.enigma.com).
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://documentation.enigma.com/reference/graphql_api/
  type: apiKey
- applies_to: Enigma MCP server (https://mcp.enigma.com/mcp)
  description: The remote MCP server authenticates with an Authorization bearer token tied to an Enigma API key. The Console "Agent tools" page emits ready-to-paste MCP client configuration with the key pre-filled. Unauthenticated calls return {"error":"invalid_token"}.
  name: BearerAuth
  scheme: bearer
  sources:
  - https://documentation.enigma.com/guides/ai-mcp
  type: http
slug: enigma-analytics-authentication
source_filename: enigma-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://documentation.enigma.com/reference/graphql_api/\ndocs: https://documentation.enigma.com/reference/graphql_api/\nsummary:\n  types: [apiKey, bearer]\n  api_key_in: [header]\n  api_key_name: x-api-key\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    applies_to: Enigma GraphQL API (https://api.enigma.com/graphql)\n    description: >-\n      All GraphQL API requests require an x-api-key request header carrying an Enigma API key\n      issued from the Enigma Console (https://console.enigma.com).\n    sources: [https://documentation.enigma.com/reference/graphql_api/]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    applies_to: Enigma MCP server (https://mcp.enigma.com/mcp)\n    description: >-\n      The remote MCP server authenticates with an Authorization bearer token tied to an Enigma API\n      key. The Console \"Agent tools\" page emits ready-to-paste\
  \ MCP client configuration with the\n      key pre-filled. Unauthenticated calls return {\"error\":\"invalid_token\"}.\n    sources: [https://documentation.enigma.com/guides/ai-mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma-analytics/refs/heads/main/authentication/enigma-analytics-authentication.yml
summary_line: apiKey/bearer · 2 schemes
tags:
- Company
- Business Data
- KYB
- Identity Verification
- Compliance
- Sanctions Screening
- GraphQL
- Fintech
- Data Enrichment
- MCP
---
