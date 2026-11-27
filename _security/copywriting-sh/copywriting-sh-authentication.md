---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Copywriting MCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copywriting MCP secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Copywriting MCP
provider_slug: copywriting-sh
scheme_count: 1
schemes:
- applies_to: https://mcp.copywriting.sh/mcp
  description: 'Per agents.md: "Header: Authorization: Bearer YOUR_PRIVATE_KEY". Buyers retrieve their private key at https://copywriting.sh/dashboard after payment. Applies to the remote MCP server https://mcp.copywriting.sh/mcp.'
  header: Authorization
  in: header
  name: bearerKey
  scheme: bearer
  type: http
slug: copywriting-sh-authentication
source_filename: copywriting-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://copywriting.sh/agents.md\ndocs: https://copywriting.sh/agents.md\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: 'Per agents.md: \"Header: Authorization: Bearer YOUR_PRIVATE_KEY\". Buyers retrieve their private key at\n    https://copywriting.sh/dashboard after payment. Applies to the remote MCP server https://mcp.copywriting.sh/mcp.'\n  applies_to: https://mcp.copywriting.sh/mcp\nnote: No OpenAPI contract is published; this profile is read from the provider's agent reference. No OAuth or scopes\n  are documented.\n"
source_yaml_url: https://artifacts.apis.io/copywriting-sh/authentication/copywriting-sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Copywriting
- MCP
- AI Agents
- Knowledge Base
- Marketing
- Content Writing
---
