---
anonymous_access: false
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Val Run Authentication
name_suffix: Authentication
oauth_flows: []
overview: Relay secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Relay
provider_slug: val-run
scheme_count: 0
schemes: []
slug: val-run-authentication
source_filename: val-run-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: a2a/val-run-agent-card.json (served card); no OpenAPI exists to run derive-authentication.py against\ndocs: null\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  open_endpoint: true\nschemes: []\nnote: >-\n  The served agent card declares no securitySchemes and no security requirements, and the endpoint\n  accepted an anonymous JSON-RPC POST (tasks/get -> -32001 Task not found, HTTP 200). The endpoint's CORS\n  policy allows an Authorization header (access-control-allow-headers includes authorization) but nothing\n  documents a credential. /.well-known/oauth-authorization-server, oauth-protected-resource and\n  openid-configuration on the endpoint host return the catch-all text banner, not metadata. Treat the\n  surface as unauthenticated; the registry's copy of the card also lists security [] and securitySchemes {}.\nx-evidence:\n  fetched: '2026-09-19'\n  anonymous_post: {url: 'https://relay2--5de8b3b2995311f1a5481607ee4eb77e.web.val.run/',\
  \ status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/val-run/refs/heads/main/authentication/val-run-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- AI Agents
- A2A
- Human-in-the-Loop
- Physical Tasks
- Errands
- Agent Network
---
