---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chilledsites Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChilledSites declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChilledSites
provider_slug: chilledsites-com
scheme_count: 1
schemes:
- applies_to: every REST call on https://api.chilledsites.com/functions/v1/api-v1, every MCP tool call (stdio server forwards both headers), and the A2A endpoint per the agent card
  gateway_note: 'The hosted MCP endpoint (/functions/v1/chatgpt-mcp) and the A2A endpoint (/functions/v1/a2a-agent) additionally return 401 {"code":"UNAUTHORIZED_NO_AUTH_HEADER"} to any request without an Authorization header — the Supabase Edge Functions gateway check — which no provider document mentions. The REST base (/functions/v1/api-v1) does NOT apply that check: an anonymous request reaches the API and gets the API''s own 401 envelope {"success":false,"error":{"code":"UNAUTHORIZED","message":"Invalid or missing API credentials"}}.'
  headers:
  - format: cs_live_... (prefix documented in agents.md and /docs/api)
    name: X-API-Key
  - format: cs_secret_... (prefix documented in agents.md and /docs/api)
    name: X-API-Secret
  id: apiKeyPair
  in: header
  issuance:
  - channel: dashboard
    docs: https://chilledsites.com/docs/api#authentication
    permissions_at_creation:
    - Read
    - Write
    - Deploy
    steps: Sign in > profile avatar > Settings > API Keys tab > Generate New API Key > name + permissions > Create; key and secret are shown once.
  - body_fields_documented:
      agents_md:
      - agent_name
      - agent_type
      - contact_email
      developers:
      - email
      - agent_name
      for_agents:
      - email
      - source
    channel: agent self-signup
    content_type: application/json
    docs: https://chilledsites.com/for-agents
    endpoint: POST https://api.chilledsites.com/functions/v1/agent-signup
    probe: GET returned 405 {"error":"Method not allowed"} with Access-Control-Allow-Methods POST, OPTIONS -- live, POST-only. Not called with POST (it would create an account).
    returns: '{ api_key, api_secret } immediately; account starts at zero tokens'
  type: apiKey
slug: chilledsites-com-authentication
source_filename: chilledsites-com-authentication.yml
source_heading: Authentication Profile
source_url: https://chilledsites.com/docs/api
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://chilledsites.com/docs/api#authentication\nsources:\n- https://chilledsites.com/docs/api\n- https://chilledsites.com/agents.md\n- https://chilledsites.com/context.md\n- https://chilledsites.com/.well-known/agent-card.json\n- https://chilledsites.com/for-agents\n- https://chilledsites.com/developers\n- npm @chilledsites/mcp-server 1.0.6 src/index.ts (the shipped client sends X-API-Key + X-API-Secret)\nnote: >-\n  No OpenAPI is published, so this profile is read from the provider's documentation and from the request\n  headers its own shipped MCP server sends. The authoritative scheme is a two-header API-key pair; two\n  older pages describe a Bearer token instead (recorded under disagreements).\nschemes:\n- id: apiKeyPair\n  type: apiKey\n  in: header\n  headers:\n  - name: X-API-Key\n    format: 'cs_live_... (prefix documented in agents.md and /docs/api)'\n  - name: X-API-Secret\n    format: 'cs_secret_... (prefix documented\
  \ in agents.md and /docs/api)'\n  applies_to: every REST call on https://api.chilledsites.com/functions/v1/api-v1, every MCP tool call (stdio server forwards both headers), and the A2A endpoint per the agent card\n  issuance:\n  - channel: dashboard\n    steps: Sign in > profile avatar > Settings > API Keys tab > Generate New API Key > name + permissions > Create; key and secret are shown once.\n    permissions_at_creation: [Read, Write, Deploy]\n    docs: https://chilledsites.com/docs/api#authentication\n  - channel: agent self-signup\n    endpoint: POST https://api.chilledsites.com/functions/v1/agent-signup\n    content_type: application/json\n    body_fields_documented:\n      agents_md: [agent_name, agent_type, contact_email]\n      for_agents: [email, source]\n      developers: [email, agent_name]\n    returns: '{ api_key, api_secret } immediately; account starts at zero tokens'\n    probe: \"GET returned 405 {\\\"error\\\":\\\"Method not allowed\\\"} with Access-Control-Allow-Methods\
  \ POST, OPTIONS -- live, POST-only. Not called with POST (it would create an account).\"\n    docs: https://chilledsites.com/for-agents\n  gateway_note: >-\n    The hosted MCP endpoint (/functions/v1/chatgpt-mcp) and the A2A endpoint (/functions/v1/a2a-agent)\n    additionally return 401 {\"code\":\"UNAUTHORIZED_NO_AUTH_HEADER\"} to any request without an Authorization\n    header — the Supabase Edge Functions gateway check — which no provider document mentions. The REST\n    base (/functions/v1/api-v1) does NOT apply that check: an anonymous request reaches the API and gets\n    the API's own 401 envelope {\"success\":false,\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Invalid or\n    missing API credentials\"}}.\nunauthenticated_response:\n  status: 401\n  body: '{\"success\":false,\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Invalid or missing API credentials\"},\"meta\":{\"timestamp\":\"2026-09-20T01:32:42.436Z\",\"version\":\"v1\"}}'\n  observed_on: GET https://api.chilledsites.com/functions/v1/api-v1/v1/websites\n\
  \  cors: 'access-control-allow-origin: *; access-control-allow-headers: x-api-key, x-api-secret, content-type, authorization; access-control-allow-methods: GET, POST, PUT, DELETE, OPTIONS'\nauthorization:\n  model: per-key permissions chosen at creation (Read, Write, Deploy); 403 FORBIDDEN when a key lacks the permission\n  billing_gate: paid routes (upload, update, deploy, and every generation) additionally require tokens or a paid account — 402 INSUFFICIENT_TOKENS otherwise (see errors/ and conventions/)\noauth2: none\nopenid_connect: none\nmutual_tls: none\ndisagreements:\n- page: https://chilledsites.com/developers\n  says: 'Authorization: Bearer YOUR_API_KEY against https://nccnasarzekslweasfpw.supabase.co/functions/v1/api-v1 with an {\"action\",\"params\"} body'\n  status: >-\n    contradicted by /docs/api, agents.md, the agent card and the shipped MCP server, all of which use the two X-API-* headers and RESTful /v1/* paths. The supabase.co host is the same backend (probed: identical\
  \ 401 envelope) but the provider's canonical host is api.chilledsites.com.\n- page: https://chilledsites.com/developer-api\n  says: 'Authorization: Bearer YOUR_API_TOKEN against https://chilledsites.com/api/v1/generate'\n  status: >-\n    dead — https://chilledsites.com/api/* returns 404 {\"code\":\"NOT_FOUND\",\"message\":\"Requested function was not found\"}; this is marketing copy for a base that does not exist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chilledsites-com/refs/heads/main/authentication/chilledsites-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Website Builder
- Artificial Intelligence
- No-Code
- Web Hosting
- Image Generation
- Video Generation
- Advertising
- MCP
- Agents
- A2A
- Small Business
- United Kingdom
---
