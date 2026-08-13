---
api_key_in:
- header
api_specs:
- filename: credo-ai-governance-platform-swagger.json
  format: json
  label: Credo AI Governance Platform API (v2)
  slug: credo-ai-governance-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/openapi/credo-ai-governance-platform-swagger.json
- filename: credo-ai-audit-logs-shadow-ai-openapi.json
  format: json
  label: Credo AI Audit Logs & Shadow AI API
  slug: credo-ai-audit-logs-shadow-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/openapi/credo-ai-audit-logs-shadow-ai-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Credo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credo AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Credo AI
provider_slug: credo-ai
scheme_count: 2
schemes:
- applied: 'globally — top-level security: [{BearerAuth: []}]'
  bearerFormat: JWT
  description: 'JWT access token obtained from POST /auth/exchange

    (CredoAIWeb.Auth.TokenController.exchange).


    Include in the Authorization header: Authorization: Bearer <token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/credo-ai-audit-logs-shadow-ai-openapi.json
  type: http
- applied: Declared in securityDefinitions but NEVER applied — the Swagger document has no top-level `security` block and no operation-level security. All 300 operations nevertheless declare a 401 AuthError response, so the requirement is real and the contract simply fails to express it.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/credo-ai-governance-platform-swagger.json
  type: apiKey
slug: credo-ai-authentication
source_filename: credo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  https://docs.sdk.credo.ai/docs/getting-started, https://api.credo.ai/openapi,\n  openapi/credo-ai-governance-platform-swagger.json, live 401 probe of\n  https://api.credo.ai/api/v2/credoai/industries on 2026-08-11\ndocs: https://docs.sdk.credo.ai/docs/getting-started\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Two-step: a long-lived tenant API token is exchanged for a short-lived JWT\n    access token, which is then sent as an Authorization: Bearer header. Every\n    request is additionally scoped by a {tenant} path segment. There are no OAuth\n    scopes and no per-token permission model in either published contract.\n  oauth2: false\n  scopes: false\n  self_serve: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT access token obtained from POST /auth/exchange\n    (CredoAIWeb.Auth.TokenController.exchange).\n\
  \n    Include in the Authorization header: Authorization: Bearer <token>\n  sources:\n  - openapi/credo-ai-audit-logs-shadow-ai-openapi.json\n  applied: 'globally — top-level security: [{BearerAuth: []}]'\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/credo-ai-governance-platform-swagger.json\n  applied: >-\n    Declared in securityDefinitions but NEVER applied — the Swagger document has\n    no top-level `security` block and no operation-level security. All 300\n    operations nevertheless declare a 401 AuthError response, so the requirement\n    is real and the contract simply fails to express it.\ntoken_exchange:\n  operation: POST /auth/exchange\n  operationId: CredoAIWeb.Auth.TokenController.exchange\n  input:\n  - tenant API token\n  - tenant identifier\n  output: JWT access token\n  documented_in: 'info.description and securitySchemes.BearerAuth description of the OpenAPI 3.0.0 document'\n  gap: >-\n    The /auth/exchange path\
  \ is described in prose and deep-linked by anchor from\n    the security scheme, but it is NOT a path in EITHER published contract. Neither\n    document describes the request body, the response shape, or the token\n    lifetime. A developer working from the specs alone cannot authenticate.\ntenancy:\n  required: true\n  placement: path segment\n  pattern: /api/v2/{tenant}\n  obtaining: >-\n    \"Your tenant identifier (contact support@credo.ai to get yours)\" — servers[]\n    variable description in the OpenAPI 3.0.0 document.\n  note: >-\n    The tenant default in the published production server is an EMPTY string, so\n    the spec cannot be used to make a call as written. The Swagger document\n    hard-codes basePath /api/v2/credoai, Credo AI's own tenant.\nsdk_configuration:\n  source: https://docs.sdk.credo.ai/docs/getting-started\n  constructor: 'Credoai(base_url=\"https://api.credo.ai\", api_key=\"your-api-key\")'\n  env_vars:\n  - CREDOAI_BASE_URL\n  - CREDOAI_API_KEY\n  key_source:\
  \ >-\n    \"You can obtain an API key from your account dashboard.\" No self-serve signup\n    exists; a tenant must be provisioned first.\n  sdk_auth_method: client.authentication.token()\n  note: >-\n    The SDK exposes the exchange as client.authentication.token() (\"Exchange API\n    Key for Access Token\"), confirming the two-step flow.\nweb_application_identity:\n  provider: Auth0\n  tenant: credoai-cs.us.auth0.com\n  discovery: https://credoai-cs.us.auth0.com/.well-known/openid-configuration\n  status: 200\n  note: >-\n    Governs the Credo AI web app and Knowledge Center login, NOT the v2 API. Its\n    scopes_supported are the stock Auth0 OIDC profile claims, not API permissions.\n    Recorded so the two identity systems are not conflated. See\n    well-known/credo-ai-well-known.yml.\nobserved:\n  url: https://api.credo.ai/api/v2/credoai/industries\n  status: 401\n  body: >-\n    {\"errors\":[{\"code\":1000,\"title\":\"Unauthenticated\",\"detail\":\"User is not\n    authenticated,\
  \ maybe invalid or expired token.\"}]}\n  fetched: '2026-08-11'\ngaps:\n- 'No /auth/exchange path in either published contract.'\n- 'No scopes, roles or permission model published for API tokens.'\n- 'Swagger securityDefinitions declared but never applied to any operation.'\n- 'No token lifetime, refresh or revocation documented.'\n- 'No self-serve key issuance — tenant provisioning goes through support@credo.ai.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/authentication/credo-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- ai-governance
- ai-risk-management
- responsible-ai
- compliance
- regulatory-technology
- model-registry
- vendor-risk
- eu-ai-act
- nist-ai-rmf
- iso-42001
- shadow-ai
- agent-governance
- audit
- json-api
- agent-skills
---
