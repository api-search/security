---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CREHQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: CREHQ declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CREHQ
provider_slug: crehq-com
scheme_count: 3
schemes:
- description: 'Every request must include a CREHQ API key, e.g. "Authorization: Bearer crehq_live_your_key_here".'
  name: bearerApiKey
  scheme: bearer
  type: http
- description: '"X-API-Key header also works" (developer hub). Sandbox /selfserve/ examples use X-API-Key.'
  header: X-API-Key
  in: header
  name: xApiKey
  type: apiKey
- description: The hosted MCP connector at https://mcp.crehq.com/mcp uses an OAuth hosted connector flow; the user authorizes the connector and pastes their CREHQ sandbox, paid or enterprise API key. No scopes are published.
  name: mcpOAuth
  type: oauth2
slug: crehq-com-authentication
source_filename: crehq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crehq.com/developers/\ndocs: https://crehq.com/developers/\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'Every request must include a CREHQ API key, e.g. \"Authorization: Bearer crehq_live_your_key_here\".'\n- name: xApiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  description: '\"X-API-Key header also works\" (developer hub). Sandbox /selfserve/ examples use X-API-Key.'\n- name: mcpOAuth\n  type: oauth2\n  description: The hosted MCP connector at https://mcp.crehq.com/mcp uses an OAuth hosted connector flow; the user authorizes the connector and pastes their CREHQ sandbox, paid or enterprise API key. No scopes are published.\nkey_types:\n- prefix: crehq_live_\n  note: Prefix shown in the developer hub example key; no test-key prefix is documented.\nkey_issuance: Free sandbox keys are delivered by email only (never returned in the HTTP response); signup is browser-only\
  \ behind Turnstile (https://crehq.com/developers/sandbox/).\naccess_model: Access follows the key; a sandbox key or research membership does not grant access to every production route.\n"
source_yaml_url: https://artifacts.apis.io/crehq-com/authentication/crehq-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Commercial Real Estate
- Location Intelligence
- Location Data
- Datasets
- Franchise Data
- Site Selection
- MCP
- Data Licensing
---
