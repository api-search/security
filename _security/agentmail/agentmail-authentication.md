---
api_key_in: []
api_specs:
- filename: agentmail-openapi-original.yml
  format: yaml
  label: AgentMail API
  slug: agentmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentmail/refs/heads/main/openapi/agentmail-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Agentmail Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentMail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgentMail
provider_slug: agentmail
scheme_count: 1
schemes:
- description: API-key bearer token (prefix am_) sent in the Authorization header. Not OAuth2 — no scopes; access is controlled by fine-grained per-key permissions.
  name: Bearer
  scheme: bearer
  sources:
  - openapi/agentmail-openapi-original.yml
  type: http
slug: agentmail-authentication
source_filename: agentmail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/agentmail-openapi-original.yml + https://docs.agentmail.to/api-reference\n  + https://docs.agentmail.to/permissions\ndocs: https://docs.agentmail.to/permissions\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  api_key_prefix: am_\n  header: 'Authorization: Bearer <api_key>'\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/agentmail-openapi-original.yml\n  description: API-key bearer token (prefix am_) sent in the Authorization header. Not\n    OAuth2 — no scopes; access is controlled by fine-grained per-key permissions.\npermissions:\n  model: fine-grained per-key permissions\n  scoping:\n  - Unrestricted (organization-wide) keys\n  - Pod-scoped keys (restricted to one pod)\n  - Inbox-scoped keys (restricted to a single inbox; added 2026-03-18)\n  docs: https://docs.agentmail.to/permissions\n  note: Permission escalation is rejected — a key cannot grant permissions it does not\n\
  \    itself hold (403 permission_escalation).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentmail/refs/heads/main/authentication/agentmail-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Email
- API
- AI Agents
- Inbox
- Messaging
- Webhooks
- WebSockets
- SMTP
- IMAP
- MCP
- Agentic
- Developer Tools
---
