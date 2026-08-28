---
api_key_in:
- header
- cookie
api_specs:
- filename: localai-api-openapi.yml
  format: yaml
  label: LocalAI API
  slug: localai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localai/refs/heads/main/openapi/localai-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Localai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LocalAI secures its APIs with apiKey, http, oauth2, and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LocalAI
provider_slug: localai
scheme_count: 1
schemes:
- declared_in_spec: true
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/localai-api-openapi.yml
  - https://localai.io/features/authentication
  type: apiKey
slug: localai-authentication
source_filename: localai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://localai.io/features/authentication\ndocs: https://localai.io/features/authentication\nspec: openapi/localai-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  - cookie\n  note: >-\n    The published Swagger 2.0 document declares only a single apiKey scheme (BearerAuth, Authorization\n    header). The documentation describes a materially larger model than the contract does: two coexisting\n    modes (legacy shared API keys and a database-backed user system) plus GitHub OAuth and generic OIDC\n    single sign-on. This artifact records the documented model; the gap between the docs and the\n    securityDefinitions block is a real contract-quality finding for the provider.\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  declared_in_spec: true\n  sources:\n  - openapi/localai-api-openapi.yml\n  - https://localai.io/features/authentication\n\
  modes:\n- id: legacy-api-key\n  name: Legacy API key authentication\n  description: >-\n    One or more shared keys configured via LOCALAI_API_KEY (comma-separated) or the equivalent CLI flag.\n    Legacy keys grant full admin access — there is no role separation. Keys can also be managed at runtime\n    through the Runtime Settings interface.\n  credential_transports:\n  - 'Authorization: Bearer <key>'\n  - 'x-api-key: <key>'\n  - 'xi-api-key: <key>'\n  - 'token cookie'\n  configuration:\n  - env: LOCALAI_API_KEY\n    description: Single key, or comma-separated list of keys.\n  - env: LOCALAI_DISABLE_API_KEY_REQUIREMENT_FOR_HTTP_GET\n    default: 'false'\n    description: Enables a GET-only compatibility override when legacy keys are configured.\n  - env: LOCALAI_HTTP_GET_EXEMPTED_ENDPOINTS\n    description: Regular expressions naming the exempt GET routes; inert unless the flag above is enabled.\n- id: user-auth\n  name: User authentication system\n  description: >-\n    A database-backed\
  \ user system (SQLite by default, PostgreSQL supported) with accounts, admin/user\n    roles, session cookies, per-user API keys, invite links and per-user token-usage accounting. The first\n    user to sign in is automatically promoted to admin.\n  enabled_by:\n  - LOCALAI_AUTH=true\n  - Setting a GitHub OAuth Client ID (auto-enables)\n  - Setting an OIDC Client ID (auto-enables)\n  roles:\n  - id: admin\n    description: >-\n      Full access, including model management, backend configuration, system settings, traces, agents and\n      user management.\n  - id: user\n    description: >-\n      Inference endpoints only — chat completions, embeddings, image/video/audio generation, TTS, MCP\n      chat, and the caller's own usage statistics.\n  registration_modes:\n  - id: open\n    description: Anyone can register and is immediately active.\n  - id: approval\n    default: true\n    description: New users land in pending status until an admin approves them; a valid invite activates immediately.\n\
  \  - id: invite\n    description: Registration requires an admin-generated invite link.\n  build_requirement: >-\n    Requires CGO and the `auth` build tag. Docker images ship with GO_TAGS=\"auth\"; a source build without\n    the tag ignores LOCALAI_AUTH entirely.\n- id: oauth-github\n  name: GitHub OAuth\n  type: oauth2\n  flow: authorizationCode\n  authorization_start: GET /api/auth/github/login\n  callback: GET /api/auth/github/callback\n  callback_url_pattern: '{LOCALAI_BASE_URL}/api/auth/github/callback'\n  configuration:\n  - env: GITHUB_CLIENT_ID\n  - env: GITHUB_CLIENT_SECRET\n  - env: LOCALAI_BASE_URL\n- id: oidc\n  name: OIDC single sign-on\n  type: openIdConnect\n  discovery: /.well-known/openid-configuration on the configured issuer\n  scopes_requested:\n  - openid\n  - profile\n  - email\n  authorization_start: GET /api/auth/oidc/login\n  callback: GET /api/auth/oidc/callback\n  callback_url_pattern: '{LOCALAI_BASE_URL}/api/auth/oidc/callback'\n  configuration:\n  - env:\
  \ LOCALAI_OIDC_ISSUER\n  - env: LOCALAI_OIDC_CLIENT_ID\n  - env: LOCALAI_OIDC_CLIENT_SECRET\n  - env: LOCALAI_BASE_URL\n  documented_providers:\n  - Keycloak\n  - Google\n  - Okta\n  - Authentik\n  - Azure AD\n- id: user-api-keys\n  name: Per-user API keys\n  description: >-\n    Authenticated users create personal keys through POST /api/auth/api-keys. A user API key inherits the\n    creating user's role, so an admin's key grants admin access.\n  management_endpoints:\n  - POST /api/auth/api-keys\n  - GET /api/auth/api-keys\n  - DELETE /api/auth/api-keys/{id}\nanonymous_surface:\n  description: >-\n    When either authentication mode is configured, the HTTP surface is private by default. Only the routes\n    below answer anonymously. If neither mode is configured the middleware does not restrict requests at all.\n  discovery:\n  - GET /.well-known/localai.json\n  - GET /api/instructions\n  - GET /api/instructions/{name}\n  - GET /swagger and GET under /swagger/\n  bootstrap:\n  - GET\
  \ /healthz\n  - GET /readyz\n  - GET /api/auth/status\n  - POST /api/auth/token-login\n  - POST /api/auth/register\n  - POST /api/auth/login\n  - GET /api/auth/github/login\n  - GET /api/auth/github/callback\n  - GET /api/auth/oidc/login\n  - GET /api/auth/oidc/callback\n  - OPTIONS under /api/auth/\n  - GET /api/branding and GET under /branding/asset/\n  overrides:\n    field: ApplicationConfig.PathWithoutAuth\n    default: empty\n    description: >-\n      Embedded deployments may add path prefixes that bypass global authentication for every HTTP method\n      below that prefix. Route-specific authorization still applies.\nauthorization:\n  model: role-based\n  admin_only_examples:\n  - GET /api/traces\n  - GET /api/traces/summary\n  - POST /api/traces/clear\n  - GET /system\n  - GET /backend/monitor\n  - POST /backend/shutdown\n  - POST /backend/load\n  - GET /api/p2p (and all /api/p2p/* routes)\n  - All /api/agent/tasks/* and /api/agent/jobs/* routes\n  - GET /models/available\n  -\
  \ GET /models/galleries\n  - GET /backends and GET /backends/available\n  user_accessible_examples:\n  - POST /v1/chat/completions\n  - POST /v1/embeddings\n  - POST /v1/completions\n  - POST /v1/images/generations\n  - POST /v1/mcp/chat/completions\n  - POST /v1/messages\n  - POST /v1/responses\n  - GET /v1/models\n  - GET /api/auth/usage\n  failure_codes:\n  - code: 401\n    condition: \"Missing or invalid credentials. Response carries the header WWW-Authenticate: Bearer.\"\n  - code: 403\n    condition: Authenticated non-admin calling an admin-only endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localai/refs/heads/main/authentication/localai-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Inference
- Self-Hosted
- Open Source
- Agents
- Model Context Protocol
- Speech
- Computer Vision
- Embeddings
- Edge Computing
---
