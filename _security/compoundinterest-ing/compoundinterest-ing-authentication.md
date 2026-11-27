---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compoundinterest-ing-openapi-generated.yml
  format: yaml
  label: Compound Interesting API
  slug: compoundinterest-ing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoundinterest-ing/openapi/_ae-authored/compoundinterest-ing-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compound Interesting Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compound Interesting declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Compound Interesting
provider_slug: compoundinterest-ing
scheme_count: 1
schemes:
- applies_to:
  - REST API https://api.compoundinterest.ing/v1
  - MCP server https://api.compoundinterest.ing/mcp
  description: Bearer API key. "Email and password. No card, no trial. The same key works for the MCP server and the HTTP API." Keys are created at https://compoundinterest.ing/account after signup.
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  name: bearer
  scheme: bearer
  type: http
slug: compoundinterest-ing-authentication
source_filename: compoundinterest-ing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compoundinterest.ing/mcp\ndocs: https://compoundinterest.ing/mcp#http\nschemes:\n- type: http\n  scheme: bearer\n  name: bearer\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  applies_to: [REST API https://api.compoundinterest.ing/v1, MCP server https://api.compoundinterest.ing/mcp]\n  description: 'Bearer API key. \"Email and password. No card, no trial. The same key works for the MCP\n    server and the HTTP API.\" Keys are created at https://compoundinterest.ing/account after signup.'\nkey_tiers:\n- free (100 units/day)\n- paid (10,000 units/day; \"Paid keys are not on sale yet\")\nunauthenticated:\n- GET /v1/demo/composite (fixed demo ticker, \"No key required\")\n- MCP tool get_demo_composite\ncli_env_var: CI_API_KEY\nobserved_401:\n  url: https://api.compoundinterest.ing/v1/composite/NVDA\n  status: 401\n  code: auth_required\n  probed: '2026-11-04'\nnote: No OAuth; no scopes. Privacy\
  \ policy states API keys are stored only as hashes.\n"
source_yaml_url: https://artifacts.apis.io/compoundinterest-ing/authentication/compoundinterest-ing-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Financial Data
- Market Intelligence
- Insider Trading
- Congressional Trades
- SEC Filings
- Institutional Holdings
- MCP
- Investing
---
