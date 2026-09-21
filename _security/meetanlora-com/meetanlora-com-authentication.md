---
anonymous_access: true
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meetanlora Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anlora secures its APIs with none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Anlora
provider_slug: meetanlora-com
scheme_count: 2
schemes:
- applies_to:
  - https://meetanlora.com/.well-known/agent-card.json (A2A agent card - four public-data skills)
  - npx -y github:Stanglovicc/anlora-mcp (MCP stdio server - four read-only tools)
  - https://meetanlora.com/.well-known/skills/index.json and the three SKILL.md files
  description: The card states "Read-only public benchmarks. No authentication required. No PII or operator-private data exposed via this agent." The MCP server runs locally with no configuration and calls no authenticated upstream.
  name: anonymous
  sources:
  - https://meetanlora.com/.well-known/agent-card.json
  - https://meetanlora.com/.well-known/mcp.json
  - https://raw.githubusercontent.com/Stanglovicc/anlora-mcp/main/README.md
  type: none
- applies_to:
  - https://meetanlora.com/api/* (private application API - not a public product)
  description: The customer dashboard (Laravel + Inertia) has an internal API under /api/ that robots.txt disallows and that answers anonymous requests with HTTP 401 {"error":{"code":"UNAUTHENTICATED","message":"Unauthenticated."}} (observed on GET /api/docs). The Privacy Policy names the session cookie anlora_session, a CSRF token, and passkeys (robots.txt Disallow /passkeys). Sign-in is at /login and /register (both 200). No API keys, tokens or OAuth clients are offered to customers or third parties anywhere in the public docs, pricing or terms - the product is sold as "no technical integration".
  name: application-session
  sources:
  - https://meetanlora.com/api/docs
  - https://meetanlora.com/robots.txt
  - https://meetanlora.com/privacy
  type: session
slug: meetanlora-com-authentication
source_filename: meetanlora-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://meetanlora.com/.well-known/agent-card.json\ndocs: https://github.com/Stanglovicc/anlora-mcp\nspec: null\nsummary:\n  types:\n  - none\n  transport: n/a - the public agent surfaces require no credential; the web application uses a browser session\n  note: >-\n    No OpenAPI exists, so derive-authentication.py has nothing to read. The profile was assembled from the agent card\n    (authentication.schemes [\"none\"], security [{scheme: none}]), the MCP manifest and repository README (stdio server,\n    no environment variables, no keys - \"Read-only. No customer data. No PII.\"), and the observed behaviour of the\n    private application API under /api/.\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - https://meetanlora.com/.well-known/agent-card.json (A2A agent card - four public-data skills)\n  - npx -y github:Stanglovicc/anlora-mcp (MCP stdio server - four read-only tools)\n  - https://meetanlora.com/.well-known/skills/index.json\
  \ and the three SKILL.md files\n  description: >-\n    The card states \"Read-only public benchmarks. No authentication required. No PII or operator-private data exposed\n    via this agent.\" The MCP server runs locally with no configuration and calls no authenticated upstream.\n  sources:\n  - https://meetanlora.com/.well-known/agent-card.json\n  - https://meetanlora.com/.well-known/mcp.json\n  - https://raw.githubusercontent.com/Stanglovicc/anlora-mcp/main/README.md\n- name: application-session\n  type: session\n  applies_to:\n  - https://meetanlora.com/api/* (private application API - not a public product)\n  description: >-\n    The customer dashboard (Laravel + Inertia) has an internal API under /api/ that robots.txt disallows and that\n    answers anonymous requests with HTTP 401 {\"error\":{\"code\":\"UNAUTHENTICATED\",\"message\":\"Unauthenticated.\"}} (observed on\n    GET /api/docs). The Privacy Policy names the session cookie anlora_session, a CSRF token, and passkeys (robots.txt\n\
  \    Disallow /passkeys). Sign-in is at /login and /register (both 200). No API keys, tokens or OAuth clients are\n    offered to customers or third parties anywhere in the public docs, pricing or terms - the product is sold as \"no\n    technical integration\".\n  sources:\n  - https://meetanlora.com/api/docs\n  - https://meetanlora.com/robots.txt\n  - https://meetanlora.com/privacy\nidentity:\n  did: did:web:meetanlora.com\n  did_document: https://meetanlora.com/.well-known/did.json\n  jwks: https://meetanlora.com/.well-known/http-message-signatures-directory\n  note: >-\n    Cryptographic identity is published for the PROVIDER (to verify claims it signs and requests it emits), not as a\n    credential a caller must present. It does not gate any surface.\noauth: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meetanlora-com/refs/heads/main/authentication/meetanlora-com-authentication.yml
summary_line: none · 2 schemes
tags:
- Creator Economy
- OnlyFans
- Agency Tooling
- Autonomous AI
- Conversational AI
- Software-as-a-Service
- Benchmarks
- Cost Modeling
- Agents
- MCP
- A2A
- Agent Skills
---
