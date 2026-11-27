---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cowerx-dev-api-tool-calls-openapi.yml
  format: yaml
  label: API Tool Calls
  slug: api-tool-calls
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cowerx-dev/openapi/cowerx-dev-api-tool-calls-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cowerx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cowerx declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cowerx
provider_slug: cowerx-dev
scheme_count: 4
schemes:
- applies_to: all API Tool Calls HTTP routes and the MCP endpoint, within the free allowance
  evidence: 'Agent tools are free: 20 calls a day per IP, no key needed.'
  name: anonymous
  type: none
- applies_to: API Tool Calls HTTP API and MCP
  evidence: The API and MCP share the free daily allowance and accept the same bearer key.
  evidence_source: https://apitoolcalls.com/agent.html
  name: bearer key
  note: 'The apitc CLI sends APITC_KEY as "Authorization: Bearer <key>". No key issuance page was found in the docs.'
  scheme: bearer
  type: http
- applies_to:
  - company_facts
  - proofread
  evidence: Send your OpenRouter key in the X-OpenRouter-Key HTTP header for MCP or POST /api/proofread . Keep keys out of tool arguments.
  evidence_source: https://apitoolcalls.com/agent.html
  header: X-OpenRouter-Key
  in: header
  name: X-OpenRouter-Key
  note: A third-party (OpenRouter) credential the caller supplies; without it a small shared daily allowance (Google Gemini) is used.
  type: apiKey
- applies_to: https://dailymd.cowerx.dev/mcp
  evidence: 'Other clients: use https://dailymd.cowerx.dev/mcp (Streamable HTTP, no auth).'
  evidence_source: https://dailymd.cowerx.dev/mcp-server/
  name: dailymd-none
  type: none
slug: cowerx-dev-authentication
source_filename: cowerx-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://apitoolcalls.com/api/\ndocs: https://apitoolcalls.com/api/\nsummary: Anonymous by default. API Tool Calls HTTP and MCP calls need no key within the free allowance (20 calls a day per IP); the API and MCP \"accept the same bearer key\", but the docs do not say how\n  a key is obtained. Two tools (company_facts, proofread) accept the caller's own OpenRouter key in an X-OpenRouter-Key header. The OpenAPI document declares no securitySchemes. The Daily Markdown MCP server\n  is \"Streamable HTTP, no auth\".\nschemes:\n- name: anonymous\n  type: none\n  applies_to: all API Tool Calls HTTP routes and the MCP endpoint, within the free allowance\n  evidence: 'Agent tools are free: 20 calls a day per IP, no key needed.'\n- name: bearer key\n  type: http\n  scheme: bearer\n  applies_to: API Tool Calls HTTP API and MCP\n  evidence: The API and MCP share the free daily allowance and accept the same bearer key.\n  evidence_source:\
  \ https://apitoolcalls.com/agent.html\n  note: 'The apitc CLI sends APITC_KEY as \"Authorization: Bearer <key>\". No key issuance page was found in the docs.'\n- name: X-OpenRouter-Key\n  type: apiKey\n  in: header\n  header: X-OpenRouter-Key\n  applies_to:\n  - company_facts\n  - proofread\n  evidence: Send your OpenRouter key in the X-OpenRouter-Key HTTP header for MCP or POST /api/proofread . Keep keys out of tool arguments.\n  evidence_source: https://apitoolcalls.com/agent.html\n  note: A third-party (OpenRouter) credential the caller supplies; without it a small shared daily allowance (Google Gemini) is used.\n- name: dailymd-none\n  type: none\n  applies_to: https://dailymd.cowerx.dev/mcp\n  evidence: 'Other clients: use https://dailymd.cowerx.dev/mcp (Streamable HTTP, no auth).'\n  evidence_source: https://dailymd.cowerx.dev/mcp-server/\nsee_also:\n- https://apitoolcalls.com/agent.html\n- https://dailymd.cowerx.dev/mcp-server/\n"
source_yaml_url: https://artifacts.apis.io/cowerx-dev/authentication/cowerx-dev-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Research
- Website Auditing
- Open Source
- MCP
- Developer Tools
---
