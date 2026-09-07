---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Meta Agent Tools API
  slug: meta-agent-tools-api
  spec_type: OpenAPI
  url: https://agentalog.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meta Agent Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meta Agent Tools secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meta Agent Tools
provider_slug: meta-agent-tools
scheme_count: 1
schemes:
- description: Guest mr_…, session sess_… or ADMIN_TOKEN.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/meta-agent-tools-openapi.json
  type: http
slug: meta-agent-tools-authentication
source_filename: meta-agent-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/meta-agent-tools-openapi.json\ndocs: https://agentalog.com/api/\nsummary:\n  types:\n  - http\n  bearer_token_kinds:\n  - guest\n  - session\n  - prepaid-credit\n  - operator-token\n  agent_payment: x402\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Guest mr_…, session sess_… or ADMIN_TOKEN.\n  sources:\n  - openapi/meta-agent-tools-openapi.json\nmodel:\n  note: >-\n    The self-describing index at https://agentalog.com/api/ documents the full tier model\n    behind the single bearer scheme (fetched 2026-09-05, HTTP 200). Tokens are prefixed by\n    kind and several headers are accepted alongside Authorization.\n  tiers:\n  - name: none\n    description: Public, no credential.\n  - name: guest\n    description: >-\n      Guest token from POST /api/guest, sent as X-Guest-Token mr_… or Authorization Bearer\n      mr_… — the identity that likes, comments and visits. A sess_… session also\
  \ works.\n  - name: session\n    description: 'Session via e-mail OTP: Authorization: Bearer sess_… (POST /api/auth/start + /api/auth/verify).'\n  - name: session_ou_x402\n    description: >-\n      Two doors to the same action — a human with a sess_… session (free, within quota) or an\n      agent paying x402 via the X-PAYMENT header ($0.10 USDC on Base). A guest token neither\n      grants nor blocks the paid path.\n  - name: credito\n    description: >-\n      Prepaid credit token as Authorization Bearer cred_… (or X-Credito header). A bearer of\n      balance, not an account — topped up once with x402 via POST /api/credito.\n  - name: token\n    description: Operator ADMIN_TOKEN or METRICS_TOKEN as Bearer; load routes also accept the enricher credential.\n  token_prefixes:\n    guest: mr_\n    session: sess_\n    credit: cred_\n  headers:\n  - Authorization\n  - X-Guest-Token\n  - X-Credito\n  - X-PAYMENT\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta-agent-tools/refs/heads/main/authentication/meta-agent-tools-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- API Registry
- Agent Registry
- MCP
- Agent Skills
- AI Agents
- Catalog
- Directory
- Search & Discovery
- x402
- Agent Payments
- Community
- UGC
---
