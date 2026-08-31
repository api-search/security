---
api_key_in:
- header
api_specs:
- filename: autogpt-external-api-openapi.json
  format: json
  label: AutoGPT External API
  slug: autogpt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-external-api-openapi.json
- filename: autogpt-agent-server-openapi.json
  format: json
  label: AutoGPT Agent Server API
  slug: autogpt-agent-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-agent-server-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: AutoGPT Platform runs two distinct authenticated surfaces on the same host. The External API (https://backend.agpt.co/external-api) is the documented, third-party-facing one and accepts either an account API key in an X-API-Key header or an OAuth 2.0 bearer token. The full Agent Server API (https://backend.agpt.co/api) is the app's own backend and is authenticated with a Supabase-issued JWT bearer; it is not documented for third parties.
kind: authentication
layout: security
method: searched
name: Autogpt Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoGPT secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AutoGPT
provider_slug: autogpt
scheme_count: 4
schemes:
- best_for: server-to-server integrations, personal scripts, backend services
  docs: https://agpt.co/docs/platform/api-and-integrations/api-guide.md
  example_request: 'curl -H "X-API-Key: YOUR_API_KEY" https://backend.agpt.co/external-api/v1/blocks

    '
  how_to_obtain: Generate an API key from AutoGPT Platform account settings. Managed through /api/api-keys on the Agent Server API (create, list, get, revoke, suspend, update permissions).
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/autogpt-external-api-openapi.json
  type: apiKey
- detail: Carries an OAuth 2.0 access token issued by https://backend.agpt.co/api/oauth/token. Tokens are prefixed agpt_xt_.
  docs: https://agpt.co/docs/platform/api-and-integrations/oauth-guide.md
  example_request: 'curl -H "Authorization: Bearer agpt_xt_..." https://backend.agpt.co/external-api/v1/blocks

    '
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/autogpt-external-api-openapi.json
  - openapi/autogpt-agent-server-openapi.json
  type: http
- bearerFormat: jwt
  detail: The default scheme on 300+ Agent Server operations. A user session JWT minted by the platform's identity provider, validated against JWT_JWKS_URL (see the self-hosting security note in the AutoGPT SECURITY.md).
  name: HTTPBearerJWT
  scheme: bearer
  sources:
  - openapi/autogpt-agent-server-openapi.json
  type: http
- detail: Shared-secret header guarding the inbound Postmark e-mail webhook. Not a consumer-facing credential.
  in: header
  name: APIKeyAuthenticator-X-Postmark-Webhook-Token
  parameter: X-Postmark-Webhook-Token
  sources:
  - openapi/autogpt-agent-server-openapi.json
  type: apiKey
slug: autogpt-authentication
source_filename: autogpt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://agpt.co/docs/platform/api-and-integrations/api-guide.md and\n  https://agpt.co/docs/platform/api-and-integrations/oauth-guide.md, reconciled\n  against the securitySchemes in openapi/autogpt-external-api-openapi.json and\n  openapi/autogpt-agent-server-openapi.json.\ndocs: https://agpt.co/docs/platform/api-and-integrations/api-guide.md\ndescription: >-\n  AutoGPT Platform runs two distinct authenticated surfaces on the same host.\n  The External API (https://backend.agpt.co/external-api) is the documented,\n  third-party-facing one and accepts either an account API key in an X-API-Key\n  header or an OAuth 2.0 bearer token. The full Agent Server API\n  (https://backend.agpt.co/api) is the app's own backend and is authenticated\n  with a Supabase-issued JWT bearer; it is not documented for third parties.\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\nsurfaces:\n  - name:\
  \ AutoGPT External API\n    base_url: https://backend.agpt.co/external-api\n    spec: openapi/autogpt-external-api-openapi.json\n    documented: true\n    console: https://backend.agpt.co/external-api/docs\n    schemes: [APIKeyHeader, HTTPBearer]\n  - name: AutoGPT Agent Server API\n    base_url: https://backend.agpt.co\n    spec: openapi/autogpt-agent-server-openapi.json\n    documented: false\n    schemes: [HTTPBearerJWT, HTTPBearer, APIKeyAuthenticator-X-Postmark-Webhook-Token]\n    note: >-\n      The first-party backend the AutoGPT web app calls. Published openly at\n      /openapi.json but not covered by the API guide; treat as internal.\nschemes:\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    sources:\n      - openapi/autogpt-external-api-openapi.json\n    how_to_obtain: >-\n      Generate an API key from AutoGPT Platform account settings. Managed\n      through /api/api-keys on the Agent Server API (create, list, get, revoke,\n      suspend,\
  \ update permissions).\n    example_request: |\n      curl -H \"X-API-Key: YOUR_API_KEY\" https://backend.agpt.co/external-api/v1/blocks\n    best_for: server-to-server integrations, personal scripts, backend services\n    docs: https://agpt.co/docs/platform/api-and-integrations/api-guide.md\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/autogpt-external-api-openapi.json\n      - openapi/autogpt-agent-server-openapi.json\n    detail: >-\n      Carries an OAuth 2.0 access token issued by\n      https://backend.agpt.co/api/oauth/token. Tokens are prefixed agpt_xt_.\n    example_request: |\n      curl -H \"Authorization: Bearer agpt_xt_...\" https://backend.agpt.co/external-api/v1/blocks\n    docs: https://agpt.co/docs/platform/api-and-integrations/oauth-guide.md\n  - name: HTTPBearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: jwt\n    sources:\n      - openapi/autogpt-agent-server-openapi.json\n    detail: >-\n      The default scheme\
  \ on 300+ Agent Server operations. A user session JWT\n      minted by the platform's identity provider, validated against JWT_JWKS_URL\n      (see the self-hosting security note in the AutoGPT SECURITY.md).\n  - name: APIKeyAuthenticator-X-Postmark-Webhook-Token\n    type: apiKey\n    in: header\n    parameter: X-Postmark-Webhook-Token\n    sources:\n      - openapi/autogpt-agent-server-openapi.json\n    detail: >-\n      Shared-secret header guarding the inbound Postmark e-mail webhook. Not a\n      consumer-facing credential.\noauth2:\n  flow: authorization_code\n  pkce_required: true\n  pkce_method: S256\n  authorization_endpoint: https://platform.agpt.co/auth/authorize\n  token_endpoint: https://backend.agpt.co/api/oauth/token\n  introspection_endpoint: https://backend.agpt.co/api/oauth/introspect\n  revocation_endpoint: https://backend.agpt.co/api/oauth/revoke\n  refresh_tokens: true\n  access_token_prefix: agpt_xt_\n  state_required: true\n  scopes: scopes/autogpt-scopes.yml\n \
  \ scope_count: 10\n  client_registration: >-\n    Manual — the docs instruct developers to contact the platform administrator\n    for a client_id, client_secret and registered redirect URIs. No public\n    dynamic client registration (RFC 7591).\n  discovery_document: >-\n    None. /.well-known/oauth-authorization-server returns 404 on every AutoGPT\n    host (probed 2026-08-29).\nunauthenticated_operations:\n  - GET /api/store/agents\n  - GET /api/store/agents/{username}/{agent_name}\n  - GET /api/store/creators\n  - GET /api/store/creators/{username}\n  - GET /api/public/shared/{share_token}\n  - GET /api/public/shared/chats/{share_token}\n  - GET /health\n  - POST /api/oauth/token\n  - POST /api/oauth/introspect\n  - POST /api/oauth/revoke\nfailure_modes:\n  - status: 401\n    body: '{\"detail\":\"Authorization header is missing\"}'\n    surface: Agent Server API\n    observed: '2026-08-29 against GET https://backend.agpt.co/api/api-keys'\n  - status: 401\n    body: '{\"detail\":\"\
  Missing authentication. Provide API key or access token.\"}'\n    surface: External API\n    observed: '2026-08-29 against GET https://backend.agpt.co/external-api/v1/blocks'\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/authentication/autogpt-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- AI Agents
- AI Automation
- Agent Platform
- Workflow-Automation
- MCP
- Open-Source
- No-Code
- LLM Orchestration
- Agent Marketplace
---
