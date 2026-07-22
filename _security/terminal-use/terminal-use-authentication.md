---
api_key_in: []
api_specs:
- filename: terminal-use-openapi-original.json
  format: json
  label: Terminal Use API
  slug: terminal-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-use/refs/heads/main/openapi/terminal-use-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Terminal Use Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal Use secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terminal Use
provider_slug: terminal-use
scheme_count: 1
schemes:
- description: Authenticate every API call with a Bearer token (API key) prefixed `tu_`. Supply it explicitly to the SDK client or via the TERMINALUSE_API_KEY environment variable. Obtain a token with `tu login` (browser flow) or from the dashboard at https://app.terminaluse.com.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.terminaluse.com/api-reference/authentication
  type: http
slug: terminal-use-authentication
source_filename: terminal-use-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.terminaluse.com/api-reference/authentication\ndocs: https://docs.terminaluse.com/concepts/keys-and-secrets\nnote: >-\n  The published OpenAPI (openapi/terminal-use-openapi-original.json) declares no\n  components.securitySchemes, so this profile is captured from the documented\n  authentication surface rather than derived from the spec.\nsummary:\n  types: [http]\n  scheme: bearer\n  token_format: \"tu_...\"\n  env_var: TERMINALUSE_API_KEY\n  base_url: https://api.terminaluse.com\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authenticate every API call with a Bearer token (API key) prefixed `tu_`.\n    Supply it explicitly to the SDK client or via the TERMINALUSE_API_KEY\n    environment variable. Obtain a token with `tu login` (browser flow) or from\n    the dashboard at https://app.terminaluse.com.\n  sources: [https://docs.terminaluse.com/api-reference/authentication]\n\
  key_types:\n- kind: API key\n  used_for: Authenticating calls to the Terminal Use API from an app, backend, or automation.\n  management: /api-reference/api-keys (list/create/get/revoke; update scopes; update sharing groups)\n  scoped: true\n  note: API keys carry scopes and can be assigned to sharing groups.\n- kind: Webhook key\n  used_for: Verifying inbound webhook delivery from Terminal Use.\n  management: tu keys (instructions/add/ls/rm); /api-reference/webhook-keys-*\n- kind: Environment secret\n  used_for: Runtime environment variables injected into a deployed agent environment (production/preview).\n  management: tu env (add/ls/get/rm/pull/import)\nrelated_endpoints:\n  oauth_tags_in_spec: [OAuth, \"CLI Authentication\", Authentication]\n  note: >-\n    The OpenAPI groups a small set of OAuth and CLI-authentication operations\n    (used by the `tu login` browser flow); end-user API access is bearer-token\n    based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-use/refs/heads/main/authentication/terminal-use-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Agents
- AI Agents
- Background Agents
- Agent Infrastructure
- Deployment
- Orchestration
- Sandboxed Compute
- Filesystems
- Developer Tools
- SDK
- CLI
---
