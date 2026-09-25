---
anonymous_access: true
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Philongevity Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phi Longevity secures its APIs with none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Phi Longevity
provider_slug: philongevity-com
scheme_count: 4
schemes:
- evidence: Anonymous POST initialize, tools/list, resources/read and tools/call all returned 200 with no credential. The provider states "No API key required for synthetic analysis" and "Stateless and carries no secrets".
  name: mcp-remote-anonymous
  origin_policy: Requests carrying a disallowed browser Origin header get HTTP 403 before any tool runs; server-to-server callers send no Origin.
  surfaces:
  - https://philongevity.com/mcp
  - https://philongevity.com/mcp-app
  type: none
- evidence: Agent card securitySchemes {} and securityRequirements [] — documented as "intentionally empty"; a consent-gated path for owner-authorized actions is in development and not live.
  name: a2a-anonymous
  surfaces:
  - https://philongevity.com/a2a
  type: none
- evidence: README — "A published, rate-limited access key is built in. If you have a dedicated key, set PHI_MCP_KEY to override it." The key authenticates the local package to Phi's gateway; the human user configures nothing.
  in: environment
  name: stdio-built-in-key
  name_of_variable: PHI_MCP_KEY
  required: false
  surfaces:
  - npx -y @phi-longevity/mcp-server
  type: apiKey
- evidence: The paid tool is gated by payment rather than identity — a base64 x402 payment payload in the `payment` parameter, per the terms returned by an unpaid call (mcp/philongevity-com-x402-payment-required.json).
  name: paid-tool-x402
  protocol: x402
  surfaces:
  - https://philongevity.com/mcp#full_prism_report
  type: payment
slug: philongevity-com-authentication
source_filename: philongevity-com-authentication.yml
source_heading: Authentication Profile
source_url: https://philongevity.com/for-agents
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://philongevity.com/for-agents\nsources:\n- https://philongevity.com/for-agents\n- https://philongevity.com/.well-known/agent-card.json\n- https://github.com/Philongevity/phi-mcp-server\nnote: >-\n  There is no OpenAPI to derive from (derive-authentication.py has no input). The profile below is read\n  from the provider's own documentation and confirmed by live anonymous calls on 2026-09-19.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  posture: Every public agent surface is unauthenticated by design.\nschemes:\n- name: mcp-remote-anonymous\n  type: none\n  surfaces: ['https://philongevity.com/mcp', 'https://philongevity.com/mcp-app']\n  evidence: Anonymous POST initialize, tools/list, resources/read and tools/call all returned 200 with no credential. The provider states \"No API key required for synthetic analysis\" and \"Stateless and carries no secrets\".\n  origin_policy: Requests carrying a disallowed\
  \ browser Origin header get HTTP 403 before any tool runs; server-to-server callers send no Origin.\n- name: a2a-anonymous\n  type: none\n  surfaces: ['https://philongevity.com/a2a']\n  evidence: Agent card securitySchemes {} and securityRequirements [] — documented as \"intentionally empty\"; a consent-gated path for owner-authorized actions is in development and not live.\n- name: stdio-built-in-key\n  type: apiKey\n  in: environment\n  name_of_variable: PHI_MCP_KEY\n  surfaces: ['npx -y @phi-longevity/mcp-server']\n  required: false\n  evidence: README — \"A published, rate-limited access key is built in. If you have a dedicated key, set PHI_MCP_KEY to override it.\" The key authenticates the local package to Phi's gateway; the human user configures nothing.\n- name: paid-tool-x402\n  type: payment\n  protocol: x402\n  surfaces: ['https://philongevity.com/mcp#full_prism_report']\n  evidence: The paid tool is gated by payment rather than identity — a base64 x402 payment payload in the\
  \ `payment` parameter, per the terms returned by an unpaid call (mcp/philongevity-com-x402-payment-required.json).\nhuman_app:\n  note: The consumer application (signup at https://philongevity.com/signup) uses account login; it is out of scope for the agent surface and the provider states agents cannot act inside a user's account today.\nidentity_of_provider:\n  agent_card_signature: ES256 JWS, kid phi-a2a-2026-08, public key at https://philongevity.com/.well-known/jwks.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philongevity-com/refs/heads/main/authentication/philongevity-com-authentication.yml
summary_line: none · 4 schemes
tags:
- Company
- Healthcare
- Health Data
- Lab Results
- Biomarkers
- Chronic Disease
- Longevity
- MCP
- A2A
- Agentic Payments
- x402
- Artificial Intelligence
---
