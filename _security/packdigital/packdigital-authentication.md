---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Packdigital Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packdigital secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Packdigital
provider_slug: packdigital
scheme_count: 2
schemes:
- applies_to:
  - https://app.packdigital.com/graphql
  in: header
  name: PackAccessToken
  parameter: Authorization
  token_types:
  - access: read-write
    name: secret
  - access: read-only
    name: public
  type: apiKey
- additional_headers:
  - x-pack-store-id
  - x-pack-content-environment-id
  applies_to:
  - https://pack-agent.packdigital.workers.dev/mcp
  name: PackMCPBearer
  parameter: Authorization
  scheme: bearer
  type: http
slug: packdigital-authentication
source_filename: packdigital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.packdigital.com/api-reference/content-management-api\ndocs: https://docs.packdigital.com/api-reference/content-management-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Token-based auth. A Pack access token is passed in the Authorization header\n    on every GraphQL request. Two token types exist: a Secret Token (read + write)\n    and a Public Token (read-only). The MCP server uses the same bearer token plus\n    a store-id header.\nschemes:\n  - name: PackAccessToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    token_types:\n      - name: secret\n        access: read-write\n      - name: public\n        access: read-only\n    applies_to:\n      - https://app.packdigital.com/graphql\n  - name: PackMCPBearer\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    additional_headers:\n      - x-pack-store-id\n      - x-pack-content-environment-id\n\
  \    applies_to:\n      - https://pack-agent.packdigital.workers.dev/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packdigital/refs/heads/main/authentication/packdigital-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Content Management
- Headless Commerce
- Shopify
- Hydrogen
- CMS
- A/B Testing
- GraphQL
- MCP
- Agents
- Storefront
---
