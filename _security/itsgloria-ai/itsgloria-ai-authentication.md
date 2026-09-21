---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: itsgloria-ai-openapi.yml
  format: yaml
  label: Gloria Data Platform REST API
  slug: gloria-data-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Itsgloria Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gloria secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gloria
provider_slug: itsgloria-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained from `/auth/verify` or `/user/api-tokens`.
  header: 'Authorization: Bearer <token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/itsgloria-ai-openapi.yml
  type: http
- description: JWT token passed as a query parameter. Equivalent to `BearerAuth`.
  in: query
  name: TokenQuery
  parameter: token
  sources:
  - openapi/itsgloria-ai-openapi.yml
  type: apiKey
slug: itsgloria-ai-authentication
source_filename: itsgloria-ai-authentication.yml
source_heading: Authentication Profile
source_url: openapi/itsgloria-ai-openapi.yml (securitySchemes BearerAuth, TokenQuery; info.description auth walkthrough)
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/itsgloria-ai-openapi.yml\ndocs: https://docs.itsgloria.ai/gloria-data-platform/api-integration/#authentication\nsources:\n- openapi/itsgloria-ai-openapi.yml (securitySchemes BearerAuth, TokenQuery; info.description auth walkthrough)\n- https://docs.itsgloria.ai/gloria-data-platform/api-integration/\n- https://docs.itsgloria.ai/gloria-data-platform/x402-integration/\n- https://www.itsgloria.ai/mcp\n- live probes of ai-hub.cryptobriefing.com, api.itsgloria.ai and mcp.itsgloria.ai on 2026-09-19\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  http_schemes:\n  - bearer (JWT)\n  issuance:\n  - siwe-wallet-signature\n  - api-token\n  - public-token\n  surfaces:\n    rest: JWT bearer / ?token= (required on every operation except getNonce, verifySignature, getPublicToken, getAvailableFeedCategories, healthCheck)\n    websocket: JWT as ?token= on the wss handshake\n    x402: no credential - X-PAYMENT header\
  \ per request (api.itsgloria.ai); /articles there wants an x-api-key header instead\n    mcp_remote: none (anonymous initialize/tools/list; paid tools hand back x402 instructions)\n    mcp_stdio: GLORIA_API_TOKEN environment variable (an API token)\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from `/auth/verify` or `/user/api-tokens`.\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - openapi/itsgloria-ai-openapi.yml\n- name: TokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: JWT token passed as a query parameter. Equivalent to `BearerAuth`.\n  sources:\n  - openapi/itsgloria-ai-openapi.yml\nflows:\n- name: SIWE wallet sign-in (EIP-4361)\n  steps:\n  - 'GET /auth/nonce -> {\"nonce\": \"...\"} (getNonce, no auth)'\n  - sign an EIP-4361 message containing the nonce with an Ethereum wallet\n  - 'POST /auth/verify {\"message\", \"signature\"} -> {\"access_token\": \"<jwt>\", \"is_admin\"\
  : false} (verifySignature)'\n  - use the JWT as Bearer or ?token=\n  docs: https://docs.itsgloria.ai/gloria-data-platform/api-integration/#wallet-authentication\n- name: API token (recommended by the docs)\n  steps:\n  - 'authenticate once (SIWE), then POST /user/api-tokens {\"name\", \"allowed_feed_categories\"} (createApiToken) - or generate in the browser at https://www.itsgloria.ai/api-keys-new'\n  - the ApiToken carries token, issued_at, expires_at and is scoped to the chosen feed categories for life\n  - GET /user/api-tokens lists, DELETE /user/api-tokens revokes\n  docs: https://docs.itsgloria.ai/gloria-data-platform/api-integration/#api-token-recommended\n- name: Public token (anonymous, read-only)\n  steps:\n  - 'GET /auth/public-token -> {\"access_token\": {\"name\": \"Auth\", \"allowed_feed_categories\": \"[]\", \"token\": \"<jwt>\"}} (getPublicToken)'\n  - roles [\"public\"], no feed permissions; observed to read GET /news on 2026-09-19\n  docs: https://docs.itsgloria.ai/gloria-data-platform/api-integration/#public-token\n\
  permissions:\n  model: feed-category scoping - each token carries allowed_feed_categories; a request for another category answers 403 Forbidden\n  categories: 19 codes from GET /available-feed-categories\nobserved:\n  missing_token: 'HTTP 401 {\"detail\":\"Missing token\"} on every gated path of ai-hub.cryptobriefing.com'\n  x402_missing_payment: 'HTTP 402 x402Version 1 body on api.itsgloria.ai/news, /recaps, /news-ticker-summary, /news-by-keyword'\noauth2: none\nopenIdConnect: none\nmutualTLS: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/authentication/itsgloria-ai-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- News
- Crypto
- Cryptocurrency
- Market Intelligence
- Sentiment Analysis
- Prediction Markets
- Artificial Intelligence
- MCP
- x402
- WebSocket
- Agents
---
