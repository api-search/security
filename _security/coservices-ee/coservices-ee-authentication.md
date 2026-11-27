---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Coservices Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coservices declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coservices
provider_slug: coservices-ee
scheme_count: 1
schemes:
- applies_to: https://mcp.coservices.ee/mcp
  description: llms.txt describes the MCP endpoint as "streamable HTTP, public read"; no credential is documented for its tools/list or tool calls.
  name: none
  type: none
slug: coservices-ee-authentication
source_filename: coservices-ee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coservices.ee/llms.txt\nschemes:\n- name: none\n  type: none\n  applies_to: https://mcp.coservices.ee/mcp\n  description: 'llms.txt describes the MCP endpoint as \"streamable HTTP, public read\"; no credential is documented for\n    its tools/list or tool calls.'\nnote: llms.txt also states agent service discovery via DNS HTTPS records `_mcp._agents.coservices.ee` -> `mcp.coservices.ee`\n  \"(authentication required)\", without documenting the scheme. No OpenAPI contract or securitySchemes are published.\n"
source_yaml_url: https://artifacts.apis.io/coservices-ee/authentication/coservices-ee-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Business Automation
- System Integrations
- Data Analytics
- Logistics
- Transport
- MCP
- AI Agents
- Estonia
---
