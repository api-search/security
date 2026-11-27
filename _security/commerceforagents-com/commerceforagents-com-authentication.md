---
anonymous_access: true
api_key_in: []
api_specs:
- filename: commerceforagents-com-mcp-api-openapi.yml
  format: yaml
  label: Commerce for Agents MCP API
  slug: commerceforagents-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerceforagents-com/openapi/commerceforagents-com-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Commerce for Agents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commerce for Agents declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Commerce for Agents
provider_slug: commerceforagents-com
scheme_count: 1
schemes:
- description: Documented as unauthenticated -- no registration, no API key, no OAuth, no bearer token.
  name: none
  source: https://commerceforagents.com/auth.md
  type: none
slug: commerceforagents-com-authentication
source_filename: commerceforagents-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commerceforagents.com/auth.md\ndocs: https://commerceforagents.com/auth.md\nname: Commerce for Agents authentication\nschemes:\n- name: none\n  type: none\n  description: Documented as unauthenticated -- no registration, no API key, no OAuth, no bearer token.\n  source: https://commerceforagents.com/auth.md\nsummary: The MCP endpoint is unauthenticated. The docs state \"There is no registration, no API key, no OAuth and no bearer token. Connect to the endpoint and call the tools.\" The OpenAPI description declares no securitySchemes.\noauth_metadata: The docs state the server publishes no OAuth Authorization Server metadata (RFC 8414) and no OAuth Protected Resource Metadata (RFC 9728), deliberately.\nuser_authorization:\n  description: What needs authorizing is human consent, not a token. Before book-contract the user must agree, in the conversation, to (1) the contract with the chosen energy provider and (2) the SEPA\
  \ direct debit mandate for the given IBAN; that agreement is passed as the `consent` field.\n  field: consent\n"
source_yaml_url: https://artifacts.apis.io/commerceforagents-com/authentication/commerceforagents-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Agentic Commerce
- MCP
- Price Comparison
- Energy
- Electricity
- Gas
- Broadband
- Mobile Plans
- eSIM
- VPN
- Germany
---
