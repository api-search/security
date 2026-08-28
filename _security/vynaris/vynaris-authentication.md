---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Vynaris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vynaris declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Vynaris
provider_slug: vynaris
scheme_count: 2
schemes:
- applies_to:
  - POST /v1/chat/completions
  - GET /v1/models
  - GET /v1/usage
  - GET /v1/ledger
  - GET /v1/ping
  format: 'Authorization: Bearer vyn_sk_live_...'
  header: Authorization
  id: bearer_api_key
  in: header
  key_length_chars: 55
  key_prefix: vyn_sk_live_
  scheme: bearer
  source: https://vynaris.com/docs#quickstart
  type: http
- applies_to:
  - POST /v1/accounts
  - GET /v1/ping
  id: anonymous
  note: 'POST /v1/accounts takes {"email": "..."} with no credential and returns a provisional key - the provider calls this "fully programmatic until money". GET /v1/ping answered 200 anonymously on 2026-08-26 with {"ok": true, "key": "invalid_or_missing"}.'
  source: https://api.vynaris.com/agents.md
  type: none
slug: vynaris-authentication
source_filename: vynaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://vynaris.com/docs\ndocs:\n- https://vynaris.com/docs#quickstart\n- https://api.vynaris.com/agents.md\n- https://vynaris.com/terms\n- https://vynaris.com/privacy\nnote: >-\n  Derived by reading the provider's published documentation, not from an\n  OpenAPI - Vynaris publishes no machine-readable contract, so\n  derive-authentication.py had no securitySchemes to read. Every statement here\n  is traceable to a docs URL below or to a live response observed on\n  2026-08-26.\nschemes:\n- id: bearer_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer vyn_sk_live_...'\n  key_prefix: vyn_sk_live_\n  key_length_chars: 55\n  applies_to:\n  - POST /v1/chat/completions\n  - GET /v1/models\n  - GET /v1/usage\n  - GET /v1/ledger\n  - GET /v1/ping\n  source: https://vynaris.com/docs#quickstart\n- id: anonymous\n  type: none\n  applies_to:\n  - POST /v1/accounts\n  - GET /v1/ping\n\
  \  note: >-\n    POST /v1/accounts takes {\"email\": \"...\"} with no credential and returns a\n    provisional key - the provider calls this \"fully programmatic until money\".\n    GET /v1/ping answered 200 anonymously on 2026-08-26 with\n    {\"ok\": true, \"key\": \"invalid_or_missing\"}.\n  source: https://api.vynaris.com/agents.md\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  model: none\n  note: >-\n    There is no OAuth scope surface. Authorization is per-key, and the levers\n    are spend caps and a provider-collection toggle rather than named scopes,\n    so no scopes/ artifact is emitted.\nkey_management:\n  storage: hashed server-side, never stored in plain text\n  visibility: shown once at creation\n  rotation: revocable per key\n  spend_caps: optional per-key spend cap\n  recommended_practice: one key per harness or machine so each can be revoked independently\n  privacy_toggle: >-\n    Each key starts metadata-only. A user may enable additional providers\
  \ on an\n    individual key, which unlocks more models and lower prices but subjects\n    request content to those providers' own retention and training terms, and\n    also causes Vynaris to store full request/response transcripts.\n  source: https://api.vynaris.com/agents.md\naccount_auth:\n  methods:\n  - email and password\n  - GitHub\n  - Google\n  console: https://app.vynaris.com/signin\n  source: https://vynaris.com/terms\nobserved:\n- url: https://api.vynaris.com/v1/models\n  status: 401\n  body: '{\"error\": {\"message\": \"Missing API key. Pass it as: Authorization: Bearer vyn_sk_live_...\", \"type\": \"auth_error\"}}'\n  fetched: '2026-08-26'\n- url: https://api.vynaris.com/v1/ping\n  status: 200\n  body: '{\"ok\": true, \"key\": \"invalid_or_missing\"}'\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vynaris/refs/heads/main/authentication/vynaris-authentication.yml
summary_line: 2 schemes
tags:
- AI
- LLM Gateway
- LLM Router / Aggregator
- Inference / Model Serving
- AI Cost Management / FinOps
- Developer Tools
- Agent Infrastructure
---
