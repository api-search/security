---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firmledger-co-ke-mcp-api-openapi.yml
  format: yaml
  label: FirmLedger MCP API
  slug: firmledger-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmledger-co-ke/openapi/firmledger-co-ke-mcp-api-openapi.yml
- filename: firmledger-co-ke-openapi-generated.yml
  format: yaml
  label: FirmLedger API
  slug: firmledger-co-ke-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmledger-co-ke/openapi/_ae-authored/firmledger-co-ke-openapi-generated.yml
auth_types: []
description: FirmLedger MCP authentication
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Firmledger Co Ke Authentication
name_suffix: Authentication
oauth_flows: []
overview: FirmLedger declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: FirmLedger
provider_slug: firmledger-co-ke
scheme_count: 3
schemes:
- evidence: 'Apps that can send a header can use the plain address https://mcp.firmledger.co.ke/mcp with Authorization: Bearer fl_live_your_key instead, which keeps the key out of URLs.'
  header: Authorization
  how_to_obtain: Generate an API key in the FirmLedger Dashboard → Developer API and use the displayed key as the bearer token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'The page shows your key once, together with your personal connector URL : connector URL https://mcp.firmledger.co.ke/mcp/fl_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
  how_to_obtain: Generate an API key in the FirmLedger Dashboard → Developer API; the key is embedded in the personal connector URL.
  location: query
  name: Connector URL key
  type: apiKey
- evidence: Use https://mcp.firmledger.co.ke/mcp with no key at all for search and basic profiles.
  how_to_obtain: None required; the endpoint is publicly accessible for limited functionality.
  location: none
  name: No authentication (public access)
  type: other
slug: firmledger-co-ke-authentication
source_filename: firmledger-co-ke-authentication.yml
source_heading: Authentication Profile
source_url: https://firmledger.co.ke/docs/mcp
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://firmledger.co.ke/docs/mcp\nsources:\n- https://firmledger.co.ke/docs/mcp\ndescription: FirmLedger MCP authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Apps that can send a header can use the plain address https://mcp.firmledger.co.ke/mcp with Authorization: Bearer fl_live_your_key\n    instead, which keeps the key out of URLs.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the FirmLedger Dashboard → Developer API and use the displayed key as the bearer token.\n- type: apiKey\n  name: Connector URL key\n  evidence: 'The page shows your key once, together with your personal connector URL : connector URL https://mcp.firmledger.co.ke/mcp/fl_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'\n  location: query\n  how_to_obtain: Generate an API key in the FirmLedger Dashboard → Developer API; the key is embedded in the\
  \ personal connector URL.\n- type: other\n  name: No authentication (public access)\n  evidence: Use https://mcp.firmledger.co.ke/mcp with no key at all for search and basic profiles.\n  location: none\n  how_to_obtain: None required; the endpoint is publicly accessible for limited functionality.\nnote: No OAuth2 flows, JWT, HMAC, or mTLS are described on the page.\ndocs: https://firmledger.co.ke/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/firmledger-co-ke/authentication/firmledger-co-ke-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Directory
- Business-Intelligence
- Kenya
- API
---
