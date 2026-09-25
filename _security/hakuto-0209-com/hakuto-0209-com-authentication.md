---
anonymous_access: false
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hakuto 0209 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: HaneruTo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HaneruTo
provider_slug: hakuto-0209-com
scheme_count: 1
schemes:
- description: b612 license key, sent verbatim in the x-b612-key header on both the A2A JSON-RPC endpoint and the MCP endpoint. Declared in the agent card as securitySchemes.b612ApiKey ("b612 license key. Contact the provider to obtain one.") and required by the card's top-level security[] on every skill. Keys are issued by the provider on contact (https://hakuto-0209.com/#contact) under a monthly licence; there is no self-serve sign-up or developer console.
  header: x-b612-key
  in: header
  key_handling: 'Per the data policy: the key is SHA-256 hashed and only the hash is sent to the licence endpoint for validation; the plaintext is never stored or logged; validation results are cached in memory for a few minutes. Usage is recorded per licence hash (counts, last use, version, access route) for licence management.'
  name: b612ApiKey
  sources:
  - https://mcp.hakuto-0209.com/.well-known/agent-card.json
  - https://mcp.hakuto-0209.com/
  - https://mcp.hakuto-0209.com/terms
  type: apiKey
slug: hakuto-0209-com-authentication
source_filename: hakuto-0209-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://mcp.hakuto-0209.com/.well-known/agent-card.json (securitySchemes + security), the provider's\n  quickstart at https://mcp.hakuto-0209.com/, the 401 body observed on https://mcp.hakuto-0209.com/a2a/v1,\n  the anonymous MCP probes on https://mcp.hakuto-0209.com/mcp, and the key-handling section of\n  https://mcp.hakuto-0209.com/terms — 2026-09-19. No OpenAPI exists to derive from.\ndocs: https://mcp.hakuto-0209.com/\nsummary:\n  types: [apiKey]\n  oauth2: false\n  oidc: false\n  keyless_tier: true\nschemes:\n- name: b612ApiKey\n  type: apiKey\n  in: header\n  header: x-b612-key\n  description: >-\n    b612 license key, sent verbatim in the x-b612-key header on both the A2A JSON-RPC endpoint and the MCP\n    endpoint. Declared in the agent card as securitySchemes.b612ApiKey (\"b612 license key. Contact the\n    provider to obtain one.\") and required by the card's top-level security[] on every skill. Keys are\n \
  \   issued by the provider on contact (https://hakuto-0209.com/#contact) under a monthly licence; there is\n    no self-serve sign-up or developer console.\n  key_handling: >-\n    Per the data policy: the key is SHA-256 hashed and only the hash is sent to the licence endpoint for\n    validation; the plaintext is never stored or logged; validation results are cached in memory for a few\n    minutes. Usage is recorded per licence hash (counts, last use, version, access route) for licence\n    management.\n  sources:\n  - https://mcp.hakuto-0209.com/.well-known/agent-card.json\n  - https://mcp.hakuto-0209.com/\n  - https://mcp.hakuto-0209.com/terms\nsurfaces:\n- surface: A2A JSON-RPC (https://mcp.hakuto-0209.com/a2a/v1)\n  requires_key: true\n  observed: >-\n    GET and an unauthenticated POST (tasks/get) both return HTTP 401 with envelope\n    {\"error\":{\"code\":\"unauthenticated\",\"message\":\"APIキー（b612 ライセンスキー）が指定されていません\",\"hint\":\n    \"ヘッダー x-b612-key に … キー無しでも次のスキルは試せます: principles\
  \ / rules …\"}}. No WWW-Authenticate\n    header is returned. The hint names a keyless tier, but the gate refused a keyless JSON-RPC request before\n    dispatch in this probe.\n- surface: MCP Streamable HTTP (https://mcp.hakuto-0209.com/mcp)\n  requires_key: partial\n  observed: >-\n    initialize, tools/list and tools/call b612_principles all answered 200 with no key. The card describes\n    principles and rules as keyless (20 req/min per IP); the remaining eight tools were not called and are\n    presumed to require the key per the quickstart's --header instruction.\nunauthenticated_response:\n  status: 401\n  content_type: application/json; charset=utf-8\n  envelope: '{\"error\":{\"code\":\"unauthenticated\",\"message\":\"<ja>\",\"hint\":\"<ja>\"}}'\nnot_present:\n- OAuth 2.0 / OIDC — no /.well-known/oauth-authorization-server, oauth-protected-resource or openid-configuration on any host\n- Self-serve sign-up, developer console or key-management UI\n- Key prefix convention (none documented)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakuto-0209-com/refs/heads/main/authentication/hakuto-0209-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agents
- MCP
- A2A
- Code Review
- Static Analysis
- Developer Tools
- Compliance
- Web Development
- Japan
- Agent-Native
---
