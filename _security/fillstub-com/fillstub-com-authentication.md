---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fillstub Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FillStub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FillStub
provider_slug: fillstub-com
scheme_count: 1
schemes:
- bearer_format: fsk_
  description: 'Authentication to the MCP server at https://mcp.fillstub.com is an HTTP Authorization header: `Authorization: Bearer fsk_...`. The token is created by the subscriber at https://fillstub.com/account. A request without a valid token sees an empty tools/list by design, because the entire content is one person''s trading history.'
  header: Authorization
  location: header
  name: Subscriber API key
  scheme: bearer
  type: http
slug: fillstub-com-authentication
source_filename: fillstub-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fillstub.com/llms-full.txt\ndocs: https://fillstub.com/llms-full.txt\nname: FillStub authentication\nschemes:\n  - type: http\n    scheme: bearer\n    bearer_format: fsk_\n    name: Subscriber API key\n    description: 'Authentication to the MCP server at https://mcp.fillstub.com is an HTTP Authorization header: `Authorization: Bearer fsk_...`. The token is created by the subscriber at https://fillstub.com/account. A request without a valid token sees an empty tools/list by design, because the entire content is one person''s trading history.'\n    location: header\n    header: Authorization\nnotes:\n  - There is no anonymous tier on MCP and no OAuth flow is documented.\n  - No OpenAPI, AsyncAPI, GraphQL, gRPC or WSDL contract is published; the single authenticated surface is the MCP JSON-RPC server.\n"
source_yaml_url: https://artifacts.apis.io/fillstub-com/authentication/fillstub-com-authentication.yml
summary_line: 1 scheme
tags:
- Options Trading
- Trading Journal
- Tax Reporting
- Section 1256
- Form 8949
- Brokerage Analytics
- P&L Analysis
- Fintech
---
