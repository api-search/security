---
api_key_in: []
api_specs:
- filename: infer-by-flow7-catalog-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Catalog API
  slug: infer-by-flow7-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-catalog-api-openapi.yml
- filename: infer-by-flow7-inference-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Inference API
  slug: infer-by-flow7-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-inference-api-openapi.yml
- filename: infer-by-flow7-status-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Status API
  slug: infer-by-flow7-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-status-api-openapi.yml
auth_types: []
description: 'Infer exposes exactly one authentication mechanism: an HTTP Bearer API key issued inside a workspace. There is no OAuth 2.0, no OIDC, no mTLS and no signed-request scheme. Two of the four published operations are deliberately unauthenticated (public catalog and public status), which is what makes the price and availability surface machine-readable without an account.'
kind: authentication
layout: security
method: searched
name: Infer By Flow7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infer by Flow7 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Infer by Flow7
provider_slug: infer-by-flow7
scheme_count: 1
schemes:
- applies_to:
  - listModels
  - createResponse
  bearer_format: Infer API key
  description: Workspace-scoped API key. Infer's spec description explicitly instructs that the key must not be placed in a URL, a prompt, a support request, or public diagnostic output; the same rule is repeated in all three published agent skills, which tell an agent to read INFER_API_KEY from the environment and never to ask a user to paste a key into chat.
  header: Authorization
  id: bearerAuth
  in: header
  scheme: bearer
  source: components.securitySchemes.bearerAuth
  type: http
  value_format: Bearer <workspace API key>
slug: infer-by-flow7-authentication
source_filename: infer-by-flow7-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  https://infer.flow7.org/docs and https://infer.flow7.org/openapi-public.json — the docs upgrade the\n  spec's single securityScheme with the key types, environments, scope name and handling rules Infer\n  publishes but does not encode in the OpenAPI.\ndescription: >-\n  Infer exposes exactly one authentication mechanism: an HTTP Bearer API key issued inside a\n  workspace. There is no OAuth 2.0, no OIDC, no mTLS and no signed-request scheme. Two of the four\n  published operations are deliberately unauthenticated (public catalog and public status), which is\n  what makes the price and availability surface machine-readable without an account.\nbase_url: https://infer.flow7.org\nschemes:\n  - id: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: Infer API key\n    in: header\n    header: Authorization\n    value_format: \"Bearer <workspace API key>\"\n    source: components.securitySchemes.bearerAuth\n\
  \    description: >-\n      Workspace-scoped API key. Infer's spec description explicitly instructs that the key must not be\n      placed in a URL, a prompt, a support request, or public diagnostic output; the same rule is\n      repeated in all three published agent skills, which tell an agent to read INFER_API_KEY from the\n      environment and never to ask a user to paste a key into chat.\n    applies_to:\n      - listModels\n      - createResponse\nkey_model:\n  issuance: >-\n    Self-serve. Create a workspace at /signup, confirm the one-time email verification link, then\n    create a key in the API keys area. Keys are shown once.\n  storage_by_provider: hashed (stated in the Privacy Notice, section 9 Security)\n  environments:\n    - name: sandbox\n      key_env_var_convention: INFER_SANDBOX_API_KEY\n      requires_funding: false\n      note: >-\n        Sandbox keys run only Infer's local demo fixture. A sandbox response carries\n        relay.environment = \"sandbox\" and relay.resolved_model_class\
  \ = \"Infer local sandbox fixture\".\n    - name: live\n      key_env_var_convention: INFER_API_KEY\n      requires_funding: true\n      note: A live key cannot send paid inference until the prepaid wallet is funded ($20 first funding).\n  scopes:\n    - name: inference:write\n      required_by:\n        - listModels\n        - createResponse\n      source: >-\n        https://infer.flow7.org/openapi-public.json — listModels description: \"The key must carry the\n        inference:write scope.\"\n      note: >-\n        This is an API-key permission scope, NOT an OAuth 2.0 scope. There is no authorization server\n        and no scope-grant flow; the scope is attached to the key when it is created.\n  spend_controls:\n    - control: per-key daily spend ceiling\n      unit: microdollars\n      note: >-\n        Enforced before a request is admitted, not after settlement. Observed in Route Note 005: a key\n        with a $0.010000 daily and monthly ceiling admitted one request and rejected\
  \ seven concurrent\n        contenders with HTTP 429 daily_budget_exceeded.\n    - control: per-key monthly spend ceiling\n      unit: microdollars\n  revocation: >-\n    Keys are revocable from the workspace. Infer's own published test records state the temporary\n    bounded keys were revoked after every task reached a terminal state.\nunauthenticated_surface:\n  - operation: getPublicCatalog\n    path: GET /api/public/catalog\n    note: Full published price catalog including per-million token rates, privacy modes and price versions.\n  - operation: getPublicStatus\n    path: GET /api/public/status\n    note: Per-service operational state and p95 latency for every published model.\nfailure_modes:\n  - status: 401\n    code: invalid_api_key\n    meaning: Missing, revoked, or invalid key.\n  - status: 403\n    meaning: The key, organization, environment, or scope cannot perform this operation.\n  - status: 402\n    code: insufficient_credits\n    meaning: The wallet cannot cover the request's\
  \ reservation.\ndocs: https://infer.flow7.org/docs\nrelated:\n  - conventions/infer-by-flow7-conventions.yml\n  - errors/infer-by-flow7-problem-types.yml\n  - scopes/infer-by-flow7-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/authentication/infer-by-flow7-authentication.yml
summary_line: 1 scheme
tags:
- AI/ML inference
- LLM API gateway
- Responses-compatible API
- Coding-agent tooling
- Developer Tools
- Usage-Based Billing
- Prepaid billing
- agent-native
- Agent Skills
- Model Routing
---
