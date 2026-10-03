---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wagerx-io-a2a-api-openapi.yml
  format: yaml
  label: WagerX A2a API
  slug: wagerx-io-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-a2a-api-openapi.yml
- filename: wagerx-io-audit-api-openapi.yml
  format: yaml
  label: WagerX Audit API
  slug: wagerx-io-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-audit-api-openapi.yml
- filename: wagerx-io-mcp-api-openapi.yml
  format: yaml
  label: WagerX MCP API
  slug: wagerx-io-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-mcp-api-openapi.yml
- filename: wagerx-io-news-api-openapi.yml
  format: yaml
  label: WagerX News API
  slug: wagerx-io-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-news-api-openapi.yml
- filename: wagerx-io-regulatory-intel-api-openapi.yml
  format: yaml
  label: WagerX Regulatory Intel API
  slug: wagerx-io-regulatory-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-regulatory-intel-api-openapi.yml
- filename: wagerx-io-slot-index-api-openapi.yml
  format: yaml
  label: WagerX Slot Index API
  slug: wagerx-io-slot-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-slot-index-api-openapi.yml
- filename: wagerx-io-trump-index-api-openapi.yml
  format: yaml
  label: WagerX Trump Index API
  slug: wagerx-io-trump-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-trump-index-api-openapi.yml
- filename: wagerx-io-well-known-api-openapi.yml
  format: yaml
  label: WagerX .well Known API
  slug: wagerx-io-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/openapi/wagerx-io-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Wagerx Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: WagerX declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: WagerX
provider_slug: wagerx-io
scheme_count: 0
schemes: []
slug: wagerx-io-authentication
source_filename: wagerx-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://wagerx.io/agent-gateway\ndocs: https://wagerx.io/agent-gateway\nspec_basis: openapi/wagerx-io-openapi.yml declares NO components.securitySchemes and no top-level security — derive-authentication.py therefore produced nothing; this profile is from the provider's docs and discovery documents.\nsummary: >-\n  Entirely anonymous, read-only public access. The Agent Gateway states \"No authentication. Rate limit: 30\n  requests/minute per IP.\" and \"FREE · NO API KEY\"; the agent card declares authentication {publicEndpoints\n  true, apiKeyRequired false} with empty securitySchemes/securityRequirements; the OpenAPI has no security\n  schemes. The same holds for the MCP endpoints (/mcp, /tech/mcp, /agents/*/mcp — tools/list accepted\n  without credentials, answering 200 or a 503 usage circuit, never 401) and the A2A endpoints.\nschemes: []\nauth_required: false\napi_keys:\n  issued: false\n  signup: none\noauth2: false\n\
  oidc: false\nmutual_tls: false\nintegrity:\n  note: >-\n    Authentication runs in the OTHER direction — the provider signs its answers so a client can verify\n    WagerX origin: agent cards carry an ES256 JWS verifiable against https://wagerx.io/.well-known/jwks.json,\n    and every A2A/MCP answer wraps data in an Ed25519-signed SignedEvidenceEnvelope verifiable against\n    https://wagerx.io/.well-known/wagerx-signing.json (canonicalise data as JSON with sorted keys, compact\n    separators, ASCII escaping; verify base64url proof.signature).\n  answer_signing_key: https://wagerx.io/.well-known/wagerx-signing.json\n  card_signing_jwks: https://wagerx.io/.well-known/jwks.json\nabuse_controls:\n  rate_limit: 30 requests/minute per IP (see rate-limits/wagerx-io-rate-limits.yml)\n  usage_circuit: MCP endpoints return JSON-RPC -32001 / HTTP 503 when the provider's \"automatic usage safety circuit\" opens (observed 2026-09-19).\n  robots: robots.txt explicitly Allows /openapi.json, /llms.txt,\
  \ the agent cards and the /api/audit/, /api/regulatory-intel, /api/news/latest paths to all agents; Disallows /api/dashboard/, /api/pwa/, /api/kings-live-bets, /chat, /dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagerx-io/refs/heads/main/authentication/wagerx-io-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Gambling
- iGaming
- Casinos
- Regulatory Intelligence
- Compliance
- Cryptocurrency
- Agents
- MCP
- A2A
- Research
---
