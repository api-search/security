---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Runtime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runtime secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runtime
provider_slug: runtime
scheme_count: 1
schemes:
- description: 'Every request must include `Authorization: Bearer runtm_sk_...`. Keys are scoped to a user and optionally to an organization. Keys carry a set of `resource:action` scopes (see scopes/runtime-scopes.yml). The raw secret is displayed only once at creation.'
  format: runtm_sk_ (opaque secret, shown once at creation)
  header: Authorization
  in: header
  name: BearerApiKey
  scheme: bearer
  sources:
  - docs.runtm.com/cloud-api/authentication
  type: http
slug: runtime-authentication
source_filename: runtime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.runtm.com/cloud-api/authentication\ndocs: https://docs.runtm.com/cloud-api/authentication\nnotes: >-\n  The Runtime Cloud API authenticates with scoped bearer-token API keys. No published OpenAPI spec\n  (the served /api-reference/openapi.json is a Mintlify sample placeholder), so this profile is\n  captured from the documented auth page rather than derived from securitySchemes.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"runtm_sk_ (opaque secret, shown once at creation)\"\n  description: >-\n    Every request must include `Authorization: Bearer runtm_sk_...`. Keys are scoped to a user and\n    optionally to an organization. Keys carry a set of `resource:action` scopes (see\n    scopes/runtime-scopes.yml). The raw secret is displayed only once at creation.\n  sources:\
  \ [docs.runtm.com/cloud-api/authentication]\norg_context:\n  header: X-Organization-Id\n  description: >-\n    Optional header to scope a request to an organization's shared resources (e.g. org_abc123).\n    Embedded in org-created keys; omitted on a personal key returns personal resources.\nkey_management:\n  creation: \"Dashboard > Settings > API Keys\"\n  presets: [Session automation, Full access, Read-only]\n  verify_endpoint: https://app.runtm.com/api/cloud/auth/verify\n  rotation: \"delete + recreate keys; role downgrades reduce a key's effective permissions at request time\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runtime/refs/heads/main/authentication/runtime-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Coding Agents
- Developer Tools
- AI Infrastructure
- Sandboxes
- Agent Orchestration
- DevOps
- Cloud
---
