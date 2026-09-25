---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kimetsu-dev-agent-gateway-openapi.yml
  format: yaml
  label: kimetsu.dev Agent Gateway
  slug: agent-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimetsu-dev/refs/heads/main/openapi/kimetsu-dev-agent-gateway-openapi.yml
auth_types:
- none
description: 'The Agent Gateway is anonymous by contract and by enforcement: the OpenAPI declares no securitySchemes and an empty security[] on every operation, the directory says "Never send credentials, cookies, private data, or authorization headers. They are rejected", and a GET carrying "Authorization: Bearer test" was answered 400 {"error":"credentials_rejected"}. derive-authentication.py therefore produced no profile (0 schemes); this file records the observed policy instead. The only authenticated surface in the product family is the self-hosted Kimetsu Remote server, which is operator-run and outside the gateway.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Kimetsu Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kimetsu secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kimetsu
provider_slug: kimetsu-dev
scheme_count: 0
schemes: []
slug: kimetsu-dev-authentication
source_filename: kimetsu-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/kimetsu-dev-agent-gateway-openapi.yml (no securitySchemes; every operation carries security []), https://agents.kimetsu.dev/\n  (authentication block), https://agents.kimetsu.dev/llms.txt (Safety boundary), https://github.com/RodCor/kimetsu.dev/blob/main/SECURITY.md,\n  https://kimetsu.dev/docs/remote/ (Kimetsu Remote bearer tokens), and a live probe on 2026-09-19.\ndocs: https://agents.kimetsu.dev/llms.txt\ndescription: 'The Agent Gateway is anonymous by contract and by enforcement: the OpenAPI declares no securitySchemes\n  and an empty security[] on every operation, the directory says \"Never send credentials, cookies, private data,\n  or authorization headers. They are rejected\", and a GET carrying \"Authorization: Bearer test\" was answered 400\n  {\"error\":\"credentials_rejected\"}. derive-authentication.py therefore produced no profile (0 schemes); this file\n  records the observed policy instead. The only\
  \ authenticated surface in the product family is the self-hosted Kimetsu\n  Remote server, which is operator-run and outside the gateway.'\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_operations: 15\n  credentialed_operations: 0\nschemes: []\npolicy:\n  credentials_rejected:\n    headers:\n    - Authorization\n    - Cookie\n    - Proxy-Authorization\n    status: 400\n    body: '{\"error\":\"credentials_rejected\",\"message\":\"This public gateway does not accept credentials. Retry without authentication or cookies.\"}'\n    observed: '2026-09-19 on GET /v1/projects'\n  rationale: SECURITY.md — the gateway is \"deliberately capability-poor\"; it constructs upstream requests from scratch\n    so caller headers never cross the trust boundary, and it is a stated security defect if any Commons surface asks\n    a participant to send credentials anywhere but api.github.com.\n  a2a_endpoint: POST /a2a/sidequest is likewise anonymous; the 1.0-negotiated Agent\
  \ Card declares securitySchemes/securityRequirements\n    for an unauthenticated interface.\nrelated_surfaces:\n  github_participation:\n    note: Proposing and voting use the participant's own GitHub credential (Issues write) sent only to api.github.com,\n      documented in the provider's separate participation contract (sidequest-openapi.json, http bearer scheme participantGitHubToken).\n      Not a credential this provider issues or receives.\n  kimetsu_remote:\n    scheme: http bearer\n    token_env: KIMETSU_REMOTE_TOKEN\n    issuance: operator-generated (--token / --tokens-file), one per teammate; writes attributed per token; rate limited\n      per token\n    transport: plain HTTP unless --features tls or a TLS proxy\n    unauthenticated: GET /healthz, GET /metrics\n    docs: https://kimetsu.dev/docs/remote/\n  kimetsu_local:\n    note: The local CLI/MCP server needs no credential for storage and retrieval; a model credential (CLAUDE_CODE_OAUTH_TOKEN,\n      Anthropic/OpenAI/Bedrock\
  \ settings) is optional and used only for `kimetsu ask`, chat and the distiller.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimetsu-dev/refs/heads/main/authentication/kimetsu-dev-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- AI Agents
- Agent Memory
- Coding Agents
- MCP
- A2A
- Developer Tools
- Open Source
- Rust
- Agent Discovery
- Public Goods
---
