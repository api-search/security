---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Delilah Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delilah declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Delilah
provider_slug: delilahusa-com
scheme_count: 4
schemes:
- applies_to: hosted MCP server https://mcp.delilahusa.com/
  description: 'Delilah API key passed as "Authorization: Bearer dk_live_YOURKEY".'
  key_prefix: dk_live_
  name: api-key-bearer
  scheme: bearer
  type: http
- applies_to: hosted MCP server https://mcp.delilahusa.com/
  description: 'Key in the server URL: https://mcp.delilahusa.com/?key=dk_live_YOURKEY'
  in: query
  name: api-key-query
  parameter: key
  type: apiKey
- applies_to: local stdio package @legislation/mcp (calls DELILAH_API_BASE, default https://api.delilahusa.com)
  description: Set DELILAH_API_KEY for your own monthly cap and for writes.
  in: environment
  name: api-key-env
  parameter: DELILAH_API_KEY
  type: apiKey
- applies_to: hosted MCP server
  description: '"The hosted server has a shared, rate-limited free tier" — no sign-in or key required; read-only.'
  name: none-free-tier
  type: none
slug: delilahusa-com-authentication
source_filename: delilahusa-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://unpkg.com/@legislation/mcp@0.7.1/README.md\ndocs: https://delilahusa.com/mcp\nnote: The Delilah developer docs (https://delilahusa.com/developers, https://delilah.tech/docs/ai-tooling) redirect to a login page, so this profile is read from the first-party npm README and the public /mcp page. No OpenAPI is publicly readable.\nschemes:\n- name: api-key-bearer\n  type: http\n  scheme: bearer\n  applies_to: hosted MCP server https://mcp.delilahusa.com/\n  description: 'Delilah API key passed as \"Authorization: Bearer dk_live_YOURKEY\".'\n  key_prefix: dk_live_\n- name: api-key-query\n  type: apiKey\n  in: query\n  parameter: key\n  applies_to: hosted MCP server https://mcp.delilahusa.com/\n  description: 'Key in the server URL: https://mcp.delilahusa.com/?key=dk_live_YOURKEY'\n- name: api-key-env\n  type: apiKey\n  in: environment\n  parameter: DELILAH_API_KEY\n  applies_to: local stdio package @legislation/mcp (calls\
  \ DELILAH_API_BASE, default https://api.delilahusa.com)\n  description: Set DELILAH_API_KEY for your own monthly cap and for writes.\n- name: none-free-tier\n  type: none\n  applies_to: hosted MCP server\n  description: '\"The hosted server has a shared, rate-limited free tier\" — no sign-in or key required; read-only.'\nkey_issuance: Keys are requested at https://delilahusa.com/developers/request (login-gated) or via https://delilahusa.com/support.\n"
source_yaml_url: https://artifacts.apis.io/delilahusa-com/authentication/delilahusa-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Legislation
- Government
- Civic Technology
- Artificial Intelligence
- Policy
- MCP
- Public Data
---
