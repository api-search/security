---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Coverage Rights Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coverage Rights declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coverage Rights
provider_slug: coverage-rights-com
scheme_count: 1
schemes:
- applies_to: https://www.coverage-rights.com/api/mcp
  client_setup: If asked for authentication, choose No sign in.
  description: The MCP server is public and unauthenticated.
  evidence: Public, read-only MCP tools. No Coverage Rights sign-in, API key or payment is required.
  name: anonymous
  type: none
slug: coverage-rights-com-authentication
source_filename: coverage-rights-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coverage-rights.com/mcp\ndocs: https://www.coverage-rights.com/mcp\nname: Coverage Rights authentication\nschemes:\n- type: none\n  name: anonymous\n  applies_to: https://www.coverage-rights.com/api/mcp\n  description: The MCP server is public and unauthenticated.\n  evidence: \"Public, read-only MCP tools. No Coverage Rights sign-in, API key or payment is required.\"\n  client_setup: \"If asked for authentication, choose No sign in.\"\nnote: No REST OpenAPI is published, so there are no declared securitySchemes; the only programmatic surface is the anonymous MCP endpoint.\n"
source_yaml_url: https://artifacts.apis.io/coverage-rights-com/authentication/coverage-rights-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Health Insurance
- Insurance Denials
- Appeals
- Prior Authorization
- Healthcare Data
- Medicare
- MCP
---
