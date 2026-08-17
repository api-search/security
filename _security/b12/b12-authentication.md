---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: B12 Authentication
name_suffix: Authentication
oauth_flows: []
overview: B12 secures its APIs with none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: B12
provider_slug: b12
scheme_count: 2
schemes:
- endpoint: https://mcp.b12.io/mcp
  evidence: POST tools/list and POST initialize both returned HTTP 200 with a complete result and no Authorization header supplied. No 401, no WWW-Authenticate, no OAuth challenge.
  name: anonymous
  sources:
  - mcp/b12-mcp.yml
  surface: mcp
  type: none
- endpoint: https://b12.io/mcp
  evidence: POST tools/list returned HTTP 200 unauthenticated.
  name: anonymous
  sources:
  - mcp/b12-mcp.yml
  surface: mcp
  type: none
slug: b12-authentication
source_filename: b12-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.b12.io/mcp\nnote: >-\n  Not derived from OpenAPI — B12 publishes none. This profile was established by\n  calling the live MCP endpoint anonymously and confirming it answers. The\n  authentication model of B12's only machine-callable surface is: there is none.\n\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  authenticated: false\n\nschemes:\n- name: anonymous\n  type: none\n  surface: mcp\n  endpoint: https://mcp.b12.io/mcp\n  sources: [mcp/b12-mcp.yml]\n  evidence: >-\n    POST tools/list and POST initialize both returned HTTP 200 with a complete\n    result and no Authorization header supplied. No 401, no WWW-Authenticate,\n    no OAuth challenge.\n- name: anonymous\n  type: none\n  surface: mcp\n  endpoint: https://b12.io/mcp\n  sources: [mcp/b12-mcp.yml]\n  evidence: POST tools/list returned HTTP 200 unauthenticated.\n\noauth_discovery:\n  oauth_authorization_server: 404\n  oauth_protected_resource:\
  \ 404\n  openid_configuration: 404\n  note: >-\n    Probed on both www.b12.io and mcp.b12.io. No OAuth or OIDC discovery\n    document is served, consistent with an unauthenticated surface. No\n    scopes/ artifact is written — there is no scope surface to record.\n\nuser_authentication:\n  note: >-\n    End users authenticate to the B12 product itself at https://b12.io/signup/\n    and https://b12.io/dashboard. That is a human web login, not an API\n    credential, and it is not reachable by an agent. The generate_website tool\n    deliberately defers it: the tool returns a signup link and the human\n    authenticates afterwards.\n\nagent_implications:\n  can_call_unauthenticated: true\n  credential_required: false\n  identity_of_caller: not established\n  note: >-\n    An agent can call generate_website with no credential and no account. B12\n    cannot attribute the call to a customer, which is why the tool returns a\n    claim link instead of a provisioned resource. This is a deliberate\
  \ design,\n    not a gap, but it does mean there is no per-caller authorization, no\n    revocation path, and no way for a customer to scope what an agent may do on\n    their behalf.\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://mcp.b12.io/mcp\n    method: POST initialize\n    http_status: 200\n    auth_supplied: none\n  - url: https://mcp.b12.io/mcp\n    method: POST tools/list\n    http_status: 200\n    auth_supplied: none\n  - url: https://mcp.b12.io/.well-known/oauth-protected-resource\n    http_status: 404\n  - url: https://mcp.b12.io/.well-known/oauth-authorization-server\n    http_status: 404\n  - url: https://www.b12.io/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b12/refs/heads/main/authentication/b12-authentication.yml
summary_line: none · 2 schemes
tags:
- Company
- Enterprise
- Website Builder
- AI
- No-Code
- Small Business
- Website Generation
- Model Context Protocol
- SEO
- Payments
---
