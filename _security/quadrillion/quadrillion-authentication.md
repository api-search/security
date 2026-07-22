---
api_key_in:
- header
api_specs:
- filename: quadrillion-cloud-openapi-original.json
  format: json
  label: Quadrillion Cloud API
  slug: quadrillion-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadrillion/refs/heads/main/openapi/quadrillion-cloud-openapi-original.json
auth_types:
- apiKey
- session
description: ''
kind: authentication
layout: security
method: searched
name: Quadrillion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quadrillion secures its APIs with apiKey and session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quadrillion
provider_slug: quadrillion
scheme_count: 2
schemes:
- description: Programmatic access to the cloud proxy and store endpoints is authorized with a Quadrillion API key. Keys are created via POST /api/keys (create_api_key_api_keys_post) — the plaintext key is returned once and cannot be retrieved again — and can be checked via POST /api/keys/validate (validate_api_key_api_keys_validate_post), listed via GET /api/keys, and revoked via DELETE /api/keys/{key_id}.
  in: header
  name: QuadrillionApiKey
  sources:
  - openapi/quadrillion-cloud-openapi-original.json
  type: apiKey
- description: The Qualia desktop app authenticates users through WorkOS-backed SSO (GET/POST /api/auth/workos/start, /callback, /discover) issuing a server session (GET /api/auth/me, /api/session, /api/session/csrf) with CSRF protection. Organization membership and provisioning are managed through the WorkOS admin portal endpoints.
  name: WorkosSSOSession
  sources:
  - openapi/quadrillion-cloud-openapi-original.json
  type: session
slug: quadrillion-authentication
source_filename: quadrillion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.quadrillion.io/settings/api-keys.md\ndocs: https://docs.quadrillion.io\nnote: >-\n  The published OpenAPI (api.quadrillion.io/openapi.json) declares no\n  components.securitySchemes, but the operation descriptions and docs state that\n  the cloud proxy routes \"require a valid Quadrillion API key,\" and the API\n  exposes first-party key management (create/validate/revoke) plus WorkOS-backed\n  SSO sessions for the desktop app.\nsummary:\n  types: [apiKey, session]\n  api_key_in: [header]\n  sso: [workos]\nschemes:\n  - name: QuadrillionApiKey\n    type: apiKey\n    in: header\n    description: >-\n      Programmatic access to the cloud proxy and store endpoints is authorized\n      with a Quadrillion API key. Keys are created via POST /api/keys\n      (create_api_key_api_keys_post) — the plaintext key is returned once and\n      cannot be retrieved again — and can be checked via POST /api/keys/validate\n     \
  \ (validate_api_key_api_keys_validate_post), listed via GET /api/keys, and\n      revoked via DELETE /api/keys/{key_id}.\n    sources: [openapi/quadrillion-cloud-openapi-original.json]\n  - name: WorkosSSOSession\n    type: session\n    description: >-\n      The Qualia desktop app authenticates users through WorkOS-backed SSO\n      (GET/POST /api/auth/workos/start, /callback, /discover) issuing a server\n      session (GET /api/auth/me, /api/session, /api/session/csrf) with CSRF\n      protection. Organization membership and provisioning are managed through\n      the WorkOS admin portal endpoints.\n    sources: [openapi/quadrillion-cloud-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadrillion/refs/heads/main/authentication/quadrillion-authentication.yml
summary_line: apiKey/session · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Research
- Data Science
- Notebooks
- LLM
- Developer Tools
- Machine Learning
---
