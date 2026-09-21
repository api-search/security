---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nefesh Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nefesh AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nefesh AI
provider_slug: nefesh-ai
scheme_count: 2
schemes:
- applies_to:
  - https://api.nefesh.ai (all /v1/* and /webhooks/* routes)
  - https://gateway.nefesh.ai (/v1/chat/completions, /v1/messages — alongside X-LLM-Key for the upstream model)
  - https://mcp.nefesh.ai/mcp (passed as a header in the MCP client config; required by get_human_state, ingest, get_trigger_memory, get_session_history)
  - https://mcp.nefesh.ai/a2a
  evidence:
  - quote: All requests require the X-Nefesh-Key header.
    source: https://nefesh.ai/docs/api
  - quote: Authentication is performed via the X-Nefesh-Key HTTP header. Each subscription provides one API key.
    source: https://nefesh.ai/terms
  - body: '{"detail":"Missing X-Nefesh-Key header."}'
    http_status: 401
    source: GET https://api.nefesh.ai/v1/state?session_id=x (no header)
  - body: '{"detail":"Invalid API key."}'
    http_status: 401
    source: 'GET https://api.nefesh.ai/v1/state?session_id=x (X-Nefesh-Key: nfsh_invalid)'
  - body: '{"detail":"Missing auth"}'
    http_status: 401
    source: GET https://api.nefesh.ai/webhooks/retries (no header)
  in: header
  issuance:
  - https://nefesh.ai/signup — email + verification link, free tier 1,000 calls/month
  - https://nefesh.ai/pricing — Solo $25/month via Stripe; one key per subscription (terms §3)
  - 'MCP self-provisioning: request_api_key(email) then poll check_api_key_status(request_id) every 10 s; key returned once, request expires after 15 minutes; disposable/placeholder emails blocked server-side'
  key_format: nfsh_... (free keys nfsh_free_...)
  name: NefeshApiKey
  parameter: X-Nefesh-Key
  type: apiKey
- applies_to:
  - https://mcp.nefesh.ai/a2a
  evidence:
  - field: authSchemes
    source: https://mcp.nefesh.ai/.well-known/agent-card.json
  - body_artifact: 'Missing API key. Provide X-Nefesh-Key header or Authorization: Bearer token. Get a free key at https://nefesh.ai/signup'
    http_status: 200
    source: POST https://mcp.nefesh.ai/a2a message/send (no credential)
  name: NefeshBearer
  note: 'The agent card''s authSchemes lists {type: http, scheme: bearer} beside the apiKey header, and the A2A README says "X-Nefesh-Key header or Authorization: Bearer token". The bearer value is the same API key, not an OAuth token.'
  scheme: bearer
  type: http
slug: nefesh-ai-authentication
source_filename: nefesh-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://nefesh.ai/docs/api\ndocs:\n- https://nefesh.ai/docs/api\n- https://nefesh.ai/docs/quickstart\n- https://nefesh.ai/docs/mcp\n- https://nefesh.ai/docs/a2a\n- https://nefesh.ai/docs/gateway\n- https://nefesh.ai/terms\nnote: >-\n  No OpenAPI is published, so this profile is written from the docs, the served agent card and live\n  unauthenticated probes rather than derived from securitySchemes. Every surface uses one credential: a per-account\n  API key sent in the X-Nefesh-Key header. Keys are prefixed nfsh_ (free-tier keys nfsh_free_); the gateway README's\n  curl examples show an older \"nk_...\" placeholder that the docs do not otherwise use. There is no OAuth 2.0, no\n  OpenID Connect, no scopes and no /.well-known/oauth-* metadata on any host (see well-known/nefesh-ai-well-known.yml),\n  so scopes/ is not emitted.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  api_key_header: X-Nefesh-Key\n  key_prefix:\
  \ nfsh_\n  bearer_accepted_on: [A2A endpoint]\n  oauth2_flows: []\n  self_provisioning: MCP tools request_api_key + check_api_key_status (no key needed; email verification link)\nschemes:\n- name: NefeshApiKey\n  type: apiKey\n  in: header\n  parameter: X-Nefesh-Key\n  applies_to:\n  - https://api.nefesh.ai (all /v1/* and /webhooks/* routes)\n  - https://gateway.nefesh.ai (/v1/chat/completions, /v1/messages — alongside X-LLM-Key for the upstream model)\n  - https://mcp.nefesh.ai/mcp (passed as a header in the MCP client config; required by get_human_state, ingest, get_trigger_memory, get_session_history)\n  - https://mcp.nefesh.ai/a2a\n  key_format: 'nfsh_... (free keys nfsh_free_...)'\n  issuance:\n  - 'https://nefesh.ai/signup — email + verification link, free tier 1,000 calls/month'\n  - 'https://nefesh.ai/pricing — Solo $25/month via Stripe; one key per subscription (terms §3)'\n  - 'MCP self-provisioning: request_api_key(email) then poll check_api_key_status(request_id) every 10 s;\
  \ key returned once, request expires after 15 minutes; disposable/placeholder emails blocked server-side'\n  evidence:\n  - {source: 'https://nefesh.ai/docs/api', quote: 'All requests require the X-Nefesh-Key header.'}\n  - {source: 'https://nefesh.ai/terms', quote: 'Authentication is performed via the X-Nefesh-Key HTTP header. Each subscription provides one API key.'}\n  - {source: 'GET https://api.nefesh.ai/v1/state?session_id=x (no header)', http_status: 401, body: '{\"detail\":\"Missing X-Nefesh-Key header.\"}'}\n  - {source: 'GET https://api.nefesh.ai/v1/state?session_id=x (X-Nefesh-Key: nfsh_invalid)', http_status: 401, body: '{\"detail\":\"Invalid API key.\"}'}\n  - {source: 'GET https://api.nefesh.ai/webhooks/retries (no header)', http_status: 401, body: '{\"detail\":\"Missing auth\"}'}\n- name: NefeshBearer\n  type: http\n  scheme: bearer\n  applies_to:\n  - https://mcp.nefesh.ai/a2a\n  note: >-\n    The agent card's authSchemes lists {type: http, scheme: bearer} beside the apiKey\
  \ header, and the A2A README says\n    \"X-Nefesh-Key header or Authorization: Bearer token\". The bearer value is the same API key, not an OAuth token.\n  evidence:\n  - {source: 'https://mcp.nefesh.ai/.well-known/agent-card.json', field: authSchemes}\n  - {source: 'POST https://mcp.nefesh.ai/a2a message/send (no credential)', http_status: 200, body_artifact: 'Missing API key. Provide X-Nefesh-Key header or Authorization: Bearer token. Get a free key at https://nefesh.ai/signup'}\ngateway_headers:\n  note: The gateway needs two credentials per request — Nefesh's and the upstream LLM provider's.\n  headers:\n  - {name: X-Nefesh-Key, required: true, description: Nefesh API key}\n  - {name: X-LLM-Key, required: true, description: 'Upstream LLM provider API key, forwarded in-memory and (per docs) never stored'}\n  - {name: X-LLM-Backend, required: false, description: 'Upstream base URL; defaults to https://api.openai.com for /v1/chat/completions and https://api.anthropic.com for /v1/messages'}\n\
  \  - {name: X-Nefesh-Subject, required: false, description: Subject id from the device registry (recommended)}\n  - {name: X-Nefesh-Session, required: false, description: Legacy session id}\nmcp_auth_model:\n  anonymous_allowed: [initialize, tools/list, resources/list, prompts/list, request_api_key, check_api_key_status]\n  key_required: [get_human_state, ingest, get_trigger_memory, get_session_history]\n  failure_mode: 'tools/call without a key returns a 200 tool result whose text is {\"error\": \"API returned 401. Check your API key and parameters.\"} with isError false — the auth failure is in-band, not a JSON-RPC error.'\nkey_handling_rules:\n  - 'Keys must not be shared, published, embedded in client-side code or transferred (terms §3).'\n  - 'Suspected compromise must be reported immediately; Nefesh may revoke compromised or misused keys without refund.'\n  - 'Subject identifiers sent with a key must be pre-hashed (SHA-256) by the customer (terms §7).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nefesh-ai/refs/heads/main/authentication/nefesh-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Biometrics
- Human State
- Stress Detection
- Affective Computing
- AI Agents
- MCP
- A2A
- LLM Gateway
- Wearables
- Digital Health
- Middleware
---
