---
api_key_in:
- header
api_specs:
- filename: lifi-openapi-original.yml
  format: yaml
  label: LI.FI API
  slug: lifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-openapi-original.yml
- filename: lifi-earn-openapi-original.yml
  format: yaml
  label: LI.FI Earn Data API
  slug: lifi-earn-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-earn-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lifi Authentication
name_suffix: Authentication
oauth_flows: []
overview: LI.FI secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LI.FI
provider_slug: lifi
scheme_count: 5
schemes:
- applies_to: LI.FI API (https://li.quest)
  in: header
  name: x-lifi-api-key
  note: Optional. Anonymous requests are served at a substantially lower rate limit.
  parameter: x-lifi-api-key
  required: false
  sources:
  - https://docs.li.fi/api-reference/rate-limits
  type: apiKey
- applies_to: LI.FI Earn API (https://earn.li.fi)
  in: header
  name: x-lifi-api-key
  parameter: x-lifi-api-key
  required: true
  sources:
  - openapi/lifi-earn-openapi-original.yml
  type: apiKey
- applies_to: Hosted MCP server (https://mcp.li.quest/mcp)
  name: Authorization
  required: false
  scheme: bearer
  sources:
  - https://docs.li.fi/mcp-server/tools
  type: http
- applies_to: Hosted MCP server (https://mcp.li.quest/mcp)
  in: header
  name: X-LiFi-Api-Key
  parameter: X-LiFi-Api-Key
  required: false
  sources:
  - https://docs.li.fi/mcp-server/tools
  type: apiKey
- applies_to: Intents Solver API (https://order.li.fi)
  in: header
  name: api-key
  note: Only the Solver API requires a key. The Intents Integrator API is open and needs no authentication.
  parameter: api-key
  required: true
  sources:
  - https://docs.li.fi/llms.txt
  type: apiKey
slug: lifi-authentication
source_filename: lifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.li.fi/api-reference/rate-limits, https://docs.li.fi/mcp-server/tools, https://docs.li.fi/cli/installation\nderived_from: openapi/lifi-earn-openapi-original.yml\ndocs: https://docs.li.fi/api-reference/rate-limits\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: >-\n    Single static API key, sent as a header. No OAuth, no OIDC, no scopes, no\n    token exchange and no per-user authorization — the key identifies the\n    integrator, not an end user. End-user authority is expressed on-chain by the\n    wallet signature, entirely outside the API.\nspec_gap_note: >-\n  The main LI.FI API OpenAPI (openapi/lifi-openapi-original.yml) declares NO\n  securitySchemes at all, even though the service accepts and rate-limits on\n  x-lifi-api-key. Only the Earn spec declares the scheme. The profile below is\n  upgraded from the documentation rather than taken from the main spec.\nschemes:\n\
  - name: x-lifi-api-key\n  type: apiKey\n  in: header\n  parameter: x-lifi-api-key\n  required: false\n  applies_to: LI.FI API (https://li.quest)\n  sources:\n  - https://docs.li.fi/api-reference/rate-limits\n  note: >-\n    Optional. Anonymous requests are served at a substantially lower rate limit.\n- name: x-lifi-api-key\n  type: apiKey\n  in: header\n  parameter: x-lifi-api-key\n  required: true\n  applies_to: LI.FI Earn API (https://earn.li.fi)\n  sources:\n  - openapi/lifi-earn-openapi-original.yml\n- name: Authorization\n  type: http\n  scheme: bearer\n  applies_to: Hosted MCP server (https://mcp.li.quest/mcp)\n  required: false\n  sources:\n  - https://docs.li.fi/mcp-server/tools\n- name: X-LiFi-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-LiFi-Api-Key\n  applies_to: Hosted MCP server (https://mcp.li.quest/mcp)\n  required: false\n  sources:\n  - https://docs.li.fi/mcp-server/tools\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  applies_to: Intents\
  \ Solver API (https://order.li.fi)\n  required: true\n  sources:\n  - https://docs.li.fi/llms.txt\n  note: >-\n    Only the Solver API requires a key. The Intents Integrator API is open and\n    needs no authentication.\nanonymous_access:\n  supported: true\n  surfaces:\n  - LI.FI API (reduced rate limit)\n  - Hosted MCP server (reduced rate limit)\n  - Intents Integrator API (no key required at all)\nkey_management:\n  obtain: https://li.fi/plans/\n  portal: https://portal.li.fi\n  env_var: LIFI_API_KEY\n  cli_commands:\n  - lifi auth show\n  - lifi auth test\n  mcp_tool: test-api-key\n  rotation_policy: null\n  scoping: >-\n    Keys are not scoped. Rate limits are calculated per key across all endpoints.\n  enforcement: >-\n    LI.FI may temporarily block keys that consistently exceed rate limits or\n    attempt to bypass limits through multiple keys or IPs.\nerrors:\n  unauthorized_code: 1010\n  unauthorized_name: UnauthorizedError\noauth2: false\nopenid_connect: false\nmutual_tls:\
  \ false\nscopes: false\nscopes_note: >-\n  No OAuth scope surface exists, so no scopes/ artifact is produced for this\n  provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/authentication/lifi-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Company
- Crypto Web3
- Blockchain
- Cross-Chain
- Bridges
- DEX Aggregation
- DeFi
- Payments
- Liquidity
- Yield
- Intents
- Agents
---
