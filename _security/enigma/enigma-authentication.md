---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Enigma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Enigma secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Enigma
provider_slug: enigma
scheme_count: 2
schemes:
- applies_to:
  - Enigma GraphQL Data API (https://api.enigma.com/graphql)
  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)
  in: header
  name: apiKey
  notes: Each request must include the x-api-key header with your API key. Keys are managed via the Enigma Console (https://console.enigma.com/) or an account representative.
  parameter_name: x-api-key
  type: apiKey
- applies_to:
  - Enigma MCP server (https://mcp.enigma.com/mcp)
  name: oauth2
  notes: The remote MCP server authenticates with OAuth 2.1 and enforces OAuth-scoped access to Enigma tools; scope reference is not publicly documented.
  type: oauth2
  version: '2.1'
slug: enigma-authentication
source_filename: enigma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://documentation.enigma.com/guides/graphql/api\ndocs: https://documentation.enigma.com/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to:\n  - Enigma GraphQL Data API (https://api.enigma.com/graphql)\n  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)\n  notes: >-\n    Each request must include the x-api-key header with your API key. Keys are managed\n    via the Enigma Console (https://console.enigma.com/) or an account representative.\n- name: oauth2\n  type: oauth2\n  version: '2.1'\n  applies_to:\n  - Enigma MCP server (https://mcp.enigma.com/mcp)\n  notes: >-\n    The remote MCP server authenticates with OAuth 2.1 and enforces OAuth-scoped access\n    to Enigma tools; scope reference is not publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma/refs/heads/main/authentication/enigma-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Business Data
- Identity Resolution
- KYB
- Compliance
- Fraud
- GraphQL
- Data Enrichment
- Financial Services
- MCP
---
