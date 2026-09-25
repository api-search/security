---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Moneyyoureowed Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Money You're Owed declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Money You're Owed
provider_slug: moneyyoureowed-com
scheme_count: 0
schemes: []
slug: moneyyoureowed-com-authentication
source_filename: moneyyoureowed-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://moneyyoureowed.com/connect\ndocs: https://moneyyoureowed.com/connect\nsummary: 'Both machine surfaces are anonymous. The /connect page states \"No API key or OAuth is required\" for the\n  MCP endpoint, and live probes confirmed it: MCP initialize/tools/list/tools/call and the A2A SendMessage call\n  all succeeded with no credential. No securitySchemes are declared in the agent card, no OAuth/OIDC discovery documents\n  exist on any host, and there is no sign-up, login or developer console.'\nschemes: []\nanonymous_access: true\nsurfaces:\n- name: MCP server\n  endpoint: https://mcp.moneyyoureowed.com/mcp\n  auth: none\n  evidence: POST tools/list and tools/call returned 200 results with no Authorization header (2026-09-19).\n- name: A2A agent\n  endpoint: https://agent.moneyyoureowed.com\n  auth: none\n  evidence: POST SendMessage returned a 200 JSON-RPC result with no Authorization header (2026-09-19); the agent\n \
  \   card declares no securitySchemes.\noauth:\n  documented: false\n  authorization_server_metadata: null\n  protected_resource_metadata: null\n  note: /.well-known/oauth-authorization-server, /oauth-protected-resource and /openid-configuration 404 on all\n    four hosts.\napi_keys:\n  documented: false\n  issuance: null\nnotes:\n- 'Abuse control is stated as rate limiting (\"Rate-limited: to control abusive traffic\") rather than credentials;\n  no limit values or headers are published (see rate-limits/).'\n- The only credentialed flow on the property is Stripe checkout for the consumer kits, which is not an API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneyyoureowed-com/refs/heads/main/authentication/moneyyoureowed-com-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Consumer Finance
- Consumer Rights
- Money Recovery
- Legal Self-Help
- Education
- Agents
- MCP
- A2A
- Agent-Native
---
