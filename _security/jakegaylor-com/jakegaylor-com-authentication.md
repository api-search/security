---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Jakegaylor Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jake Gaylor declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Jake Gaylor
provider_slug: jakegaylor-com
scheme_count: 0
schemes: []
slug: jakegaylor-com-authentication
source_filename: jakegaylor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live probes 2026-09-19 of https://ai.jakegaylor.com/mcp and /a2a; agent card securitySchemes; https://github.com/jhgaylor/ai-jakegaylor-com\n  README\nsummary:\n  types: []\n  public_surface: Everything. MCP initialize/tools/list/resources/list/prompts/list and A2A message/send, SendMessage\n    and tasks/get all answered with no credential on 2026-09-19.\n  oauth2: false\n  oidc: false\n  api_key: false\n  mutual_tls: false\nschemes: []\nsession:\n  mcp: 'Stateful Streamable HTTP: initialize returns an mcp-session-id response header that MUST be echoed on every\n    later request; a call without it is rejected with JSON-RPC -32000 \"session ID required or initialization expected\"\n    (HTTP 400). This is transport state, not authentication.'\n  a2a: None. The 1.0 card declares securitySchemes {} and securityRequirements []; the 0.3 body declares none.\nidentity_signals:\n  caller_context: The provider's llms.txt asks callers\
  \ to say who they are via an optional caller_context argument\n    (\"It is logged and read by Jake. Identified callers hear back faster.\") - a voluntary attribution convention,\n    not an auth scheme, and not present in the live tool schemas (see mcp/jakegaylor-com-mcp.yml).\n  card_signature: The agent card is JWS-signed (ES256, kid jakegaylor-a2a-2026) with keys at /.well-known/jwks.json\n    - that authenticates the CARD to the caller, not the caller to the server.\nwell_known:\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  openid_configuration: 404\n  note: Consistent with an anonymous surface; RFC 9728 metadata is not expected where no resource is protected.\ndocs:\n- https://ai.jakegaylor.com/\n- https://github.com/jhgaylor/ai-jakegaylor-com\nnote: 'An anonymous agent surface by design: the operator is a job candidate who wants recruiters'' agents to reach\n  him without friction. Guardrails sit on the side-effecting operations instead (explicit BOOK:/CONTACT:\
  \ prefixes\n  on A2A, pending human confirmation on bookings, a daily booking-attempt cap) - see conventions/jakegaylor-com-conventions.yml.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jakegaylor-com/refs/heads/main/authentication/jakegaylor-com-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Agents
- AI Agents
- A2A
- MCP
- Hiring
- Recruiting
- Resume
- Scheduling
- Personal Agent
---
