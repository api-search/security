---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: P0Stman Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: p0stman declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: p0stman
provider_slug: p0stman-com
scheme_count: 1
schemes:
- applies_to:
    a2a:
    - GET /api/agent (card)
    - POST /api/agent (JSON-RPC)
    json:
    - GET /api/ai/context
    - GET /api/ai/services
    - GET /api/ai/portfolio
    mcp:
    - initialize
    - tools/list
    - tools/call book_discovery_call
    - tools/call submit_inquiry
    - tools/call get_services
    - tools/call get_portfolio
    - tools/call search_content
  detail: 'No Authorization header, API key, cookie or session is required or documented. CORS is open (access-control-allow-origin: *). Caller identity for the write tools is the name/email in the arguments, which p0stman receives as an enquiry.'
  id: none
  observed:
  - method: POST tools/list
    status: 200
    url: https://p0stman.com/api/mcp
    www_authenticate: null
  - method: POST tools/call get_services
    status: 200
    url: https://p0stman.com/api/mcp
  - method: POST tasks/get
    not an auth challenge: null
    note: JSON-RPC -32602 shape error - a validation failure
    status: 400
    url: https://p0stman.com/api/agent
  - method: GET
    status: 200
    url: https://p0stman.com/api/ai/context
  type: none
slug: p0stman-com-authentication
source_filename: p0stman-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\ndocs: https://p0stman.com/agents.md\nsource: >-\n  https://p0stman.com/.well-known/agent-card.json (authentication.schemes), anonymous POSTs to\n  https://p0stman.com/api/mcp and https://p0stman.com/api/agent, anonymous GETs to /api/ai/context,\n  /api/ai/services and /api/ai/portfolio, https://p0stman.com/agents.md and the /.well-known/ probe - all\n  2026-09-19. derive-authentication.py was not run: there is no OpenAPI to derive from.\nsummary: >-\n  Every public machine surface p0stman exposes is anonymous. The MCP server answered initialize, tools/list\n  and a tools/call with no credential and no WWW-Authenticate challenge; the A2A card declares\n  authentication.schemes [\"None\"] and the task endpoint accepted an anonymous JSON-RPC POST; the three\n  /api/ai JSON endpoints return 200 to a bare GET; agents.md documents no key, token or sign-up anywhere.\n  There is no OAuth authorization server, no OpenID configuration, no protected-resource\
  \ metadata and no\n  developer sign-up - consistent with a surface whose only writes are \"send us an enquiry\". The two write\n  tools identify the caller by the name and email supplied in the tool arguments, not by any credential.\nschemes:\n- id: none\n  type: none\n  applies_to:\n    mcp: [initialize, tools/list, tools/call book_discovery_call, tools/call submit_inquiry, tools/call get_services, tools/call get_portfolio, tools/call search_content]\n    a2a: [GET /api/agent (card), POST /api/agent (JSON-RPC)]\n    json: [GET /api/ai/context, GET /api/ai/services, GET /api/ai/portfolio]\n  detail: >-\n    No Authorization header, API key, cookie or session is required or documented. CORS is open\n    (access-control-allow-origin: *). Caller identity for the write tools is the name/email in the\n    arguments, which p0stman receives as an enquiry.\n  observed:\n  - {url: https://p0stman.com/api/mcp, method: POST tools/list, status: 200, www_authenticate: null}\n  - {url: https://p0stman.com/api/mcp,\
  \ method: POST tools/call get_services, status: 200}\n  - {url: https://p0stman.com/api/agent, method: POST tasks/get, status: 400, note: JSON-RPC -32602 shape error - a validation failure, not an auth challenge}\n  - {url: https://p0stman.com/api/ai/context, method: GET, status: 200}\noauth:\n  authorization_server_metadata: {url: https://p0stman.com/.well-known/oauth-authorization-server, status: 404}\n  protected_resource_metadata: {url: https://p0stman.com/.well-known/oauth-protected-resource, status: 404}\n  openid_configuration: {url: https://p0stman.com/.well-known/openid-configuration, status: 404}\n  dynamic_client_registration: false\n  scopes: none - see conformance; no scopes artifact is written because no OAuth surface exists\na2a_card_declaration:\n  field: authentication.schemes\n  value: ['None']\n  note: pre-0.3 field name; A2A 1.0.0 uses securitySchemes / security\ngated_surfaces:\n  note: >-\n    robots.txt disallows /api/zero-chat, /api/clawos-chat, /api/clawos-poll,\
  \ /api/gemini-session, /api/admin,\n    /api/cron, /api/track and /api/indexnow. These back the site's own chat/voice widgets and operations and\n    are not published for third parties; they were not probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p0stman-com/refs/heads/main/authentication/p0stman-com-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- MCP
- A2A
- Agentic Web
- Voice AI
- AI Automation
- Product Studio
- Software Development
- Consulting
- United Kingdom
---
