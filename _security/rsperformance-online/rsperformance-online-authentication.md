---
anonymous_access: true
api_key_in: []
api_specs:
- filename: rsperformance-online-ai-gateway-openapi.yml
  format: yaml
  label: RS Performance AI Gateway API
  slug: rs-performance-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/openapi/rsperformance-online-ai-gateway-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Rsperformance Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: RS Performance secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RS Performance
provider_slug: rsperformance-online
scheme_count: 1
schemes:
- name: none
  sources:
  - openapi/rsperformance-online-ai-gateway-openapi.yml
  - a2a/rsperformance-online-agent-card.json
  - well-known/rsperformance-online-agents.json
  - well-known/rsperformance-online-ai-plugin.json
  surfaces:
  - declared_in: a2a/rsperformance-online-agent-card.json (securitySchemes {})
    surface: A2A JSON-RPC 2.0 — POST https://rsperformance.online/
    verified: tasks/list and an unknown-method probe answered 200 with no credential
  - declared_in: well-known/rsperformance-online-legacy-agent.json (authentication.schemes ["none"])
    surface: A2A HTTP+JSON — https://rsperformance.online/message:send, /message:stream, /tasks
    verified: GET /tasks answered 200 application/json with no credential
  - declared_in: openapi/rsperformance-online-ai-gateway-openapi.yml (no securitySchemes, no security[])
    surface: REST gateway — https://ai.rsperformance.online/api/search
    verified: POST returned 200 with hits for {"query":"P0299","limit":2}
  - declared_in: llms.txt ("Public semantic knowledge search")
    surface: REST apex — GET https://rsperformance.online/api/knowledge/search
    verified: 200 with X-RateLimit-Limit 30
  - declared_in: well-known/rsperformance-online-ai-plugin.json (auth.type none, has_user_authentication false)
    surface: MCP — https://mcp.rs3d.pl/
    verified: initialize, tools/list, resources/list, prompts/list all 200 with no credential; /.well-known/oauth-protected-resource 404
  type: none
slug: rsperformance-online-authentication
source_filename: rsperformance-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nsource: >-\n  Provider statements on 2026-09-19 — agent card securitySchemes {} / securityRequirements [],\n  legacy agent.json authentication.schemes [\"none\"], agents.json authentication.type \"none\",\n  ai-plugin.json auth.type \"none\", security.txt \"Public surfaces, no auth required\" — cross-checked\n  against live anonymous calls that succeeded on every surface.\ndocs: https://rsperformance.online/.well-known/agents.json\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_surfaces: [a2a-jsonrpc, a2a-http-json, rest-gateway, rest-apex-knowledge-search, mcp-diagnosta-rs]\n  gated_surfaces: []\n  note: >-\n    Every published surface is anonymous by design and says so in its own manifest. The OpenAPI\n    declares no securitySchemes and no security requirement; the A2A card declares an empty\n    securitySchemes object; the MCP server accepted initialize and tools/list with no credential\
  \ and\n    publishes no RFC 9728 protected-resource metadata. Access control is fair-use rate limiting\n    (rate-limits/rsperformance-online-rate-limits.yml) and a documented bot allowlist in robots.txt.\n    The provider's own customer (/klient/login) and fleet (/flota/login) portals are session-login\n    web apps, disallowed in robots.txt, and are not API authentication.\nschemes:\n  - name: none\n    type: none\n    surfaces:\n      - surface: A2A JSON-RPC 2.0 — POST https://rsperformance.online/\n        declared_in: a2a/rsperformance-online-agent-card.json (securitySchemes {})\n        verified: tasks/list and an unknown-method probe answered 200 with no credential\n      - surface: A2A HTTP+JSON — https://rsperformance.online/message:send, /message:stream, /tasks\n        declared_in: well-known/rsperformance-online-legacy-agent.json (authentication.schemes [\"none\"])\n        verified: GET /tasks answered 200 application/json with no credential\n      - surface: REST gateway\
  \ — https://ai.rsperformance.online/api/search\n        declared_in: openapi/rsperformance-online-ai-gateway-openapi.yml (no securitySchemes, no security[])\n        verified: POST returned 200 with hits for {\"query\":\"P0299\",\"limit\":2}\n      - surface: REST apex — GET https://rsperformance.online/api/knowledge/search\n        declared_in: llms.txt (\"Public semantic knowledge search\")\n        verified: 200 with X-RateLimit-Limit 30\n      - surface: MCP — https://mcp.rs3d.pl/\n        declared_in: well-known/rsperformance-online-ai-plugin.json (auth.type none, has_user_authentication false)\n        verified: initialize, tools/list, resources/list, prompts/list all 200 with no credential; /.well-known/oauth-protected-resource 404\n    sources: [openapi/rsperformance-online-ai-gateway-openapi.yml, a2a/rsperformance-online-agent-card.json, well-known/rsperformance-online-agents.json, well-known/rsperformance-online-ai-plugin.json]\ncrawler_identity:\n  robots_txt: https://rsperformance.online/robots.txt\n\
  \  note: >-\n    robots.txt enumerates named AI/search user agents (Applebot, Claude-SearchBot, DuckAssistBot,\n    Firecrawl, ...) with Allow: / and a shared Disallow set (/admin, /klient, /flota, /livewire,\n    /storage, /vendor); the gateway agent.json names ClaudeBot as a blocked family on canonical hosting\n    and offers ai.rsperformance.online as the rescue lane. Identification is by User-Agent string only —\n    no Web Bot Auth / HTTP Message Signatures.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/authentication/rsperformance-online-authentication.yml
summary_line: none · 1 scheme
tags:
- Automotive
- Auto Repair
- Vehicle Diagnostics
- OBD-II
- Fault Codes
- Knowledge Base
- Semantic Search
- A2A
- MCP
- agent-native
- Local Business
- Poland
---
