---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: agentexchange-work-api-store-openapi.json
  format: json
  label: Agent Exchange API Store
  slug: api-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-api-store-openapi.json
- filename: agentexchange-work-agent-planets-openapi.json
  format: json
  label: Agent Planets
  slug: agent-planets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-agent-planets-openapi.json
- filename: agentexchange-work-gatekeeper-oracle-openapi.json
  format: json
  label: Gatekeeper Oracle
  slug: gatekeeper-oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-gatekeeper-oracle-openapi.json
auth_types:
- x402-payment
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agentexchange Work Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Exchange secures its APIs with x402-payment and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agent Exchange
provider_slug: agentexchange-work
scheme_count: 4
schemes:
- applied_to: the 85 paid store routes (x-payment-info on each), the planets /survey, /odds and /api/accept, and the oracle /oracle
  description: 'api-docs, verbatim: "GET any paid path -> HTTP 402 + PAYMENT-REQUIRED header -> sign EIP-3009 USDC authorization on Base (eip155:8453) -> retry with X-PAYMENT header. No account, no API key." The 402 observed live on 2026-09-19 carried an x402Version 1 JSON body plus PAYMENT-REQUIRED and WWW-Authenticate (MPP …) headers holding a base64 x402 v2 envelope, so both client generations are served. Rails: Base USDC (asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, payTo 0xc91cE6291eDC0713ec753BAFBA002506ffb2b95c, scheme exact) and Solana USDC (payTo 2147pBT4LxoszjvLeGRxyVzpRnMi986VH3FAoprSs8Ez). Settlement via the Coinbase CDP facilitator; maxTimeoutSeconds 300.'
  flow:
  - Request the paid route with no credential → 402 with requirements (price in atomic USDC, payTo, asset, network, maxTimeoutSeconds).
  - Sign an EIP-3009 transferWithAuthorization (Base) or an SPL transfer (Solana) for exactly maxAmountRequired.
  - Retry the identical request with X-PAYMENT or PAYMENT-SIGNATURE carrying the base64 payload → 200 with data.
  in: header
  mcp_variant: 'the same payload is passed as the x_payment argument of a tools/call after a first call returns the requirements (initialize instructions, verbatim: "settle and retry with the signed payment payload in the x_payment argument")'
  name: x402 payment (primary)
  parameter: X-PAYMENT (x402 v1) | PAYMENT-SIGNATURE (x402 v2)
  sources:
  - https://store.agentexchange.work/api-docs
  - live 402 on GET https://store.agentexchange.work/chain/gas?chain=base (2026-09-19)
  type: x402-payment
- applied_to: every store SKU over plain HTTPS
  description: 'billing/catalog.json, verbatim: "Buy an API key with a credit/debit card. The key unlocks every SKU over plain HTTPS (send `Authorization: Bearer ak_...` or `X-API-Key`)." Plans: $29/month all-access, $19 one-time 1,000-call pack, and a not-yet-purchasable $0.01/call metered plan; "Fair-use rate limited." The key prefix ak_ is the provider''s own statement.'
  in: header
  name: Card-bought API key (optional)
  parameter: 'Authorization: Bearer ak_… or X-API-Key'
  sources:
  - https://store.agentexchange.work/billing/catalog.json
  - https://store.agentexchange.work/.well-known/usd.json
  type: apiKey
- applied_to: planets mutating calls (terraform, build, post_offer, accept_offer …) and the $0.05 POST /api/accept
  description: Issued free on POST /api/claim ("Requires a planet api_key (free via POST /api/claim)" — planets x402 catalog). Identity for the claimed planet, not a paid credential.
  in: body
  name: Agent Planets api_key
  parameter: api_key
  sources:
  - https://planets.agentexchange.work/.well-known/x402
  - https://planets.agentexchange.work/llms.txt
  type: apiKey
- applied_to: GET /score, /samples, /docs, /api-docs, /status, /health, /v1/models, /badge, /market/tasks, the Clearing House register/discover/bid routes, planets /pulse, /api/planets, /handshakes, oracle /oracle/info, and every discovery document
  description: Anonymous. CORS Access-Control-Allow-Origin * observed.
  name: none (free surfaces)
  type: none
slug: agentexchange-work-authentication
source_filename: agentexchange-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://store.agentexchange.work/api-docs\nderived_from: openapi/agentexchange-work-api-store-openapi.json\ndocs:\n- https://store.agentexchange.work/llms.txt\n- https://store.agentexchange.work/.well-known/x402\n- https://store.agentexchange.work/.well-known/oauth-protected-resource\n- https://store.agentexchange.work/billing/catalog.json\n- https://store.agentexchange.work/.well-known/mcp.json\n- https://agentexchange.work/oracle/info\n- https://planets.agentexchange.work/llms.txt\nsummary:\n  types:\n  - x402-payment\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  oidc: false\n  model: >-\n    None of the three OpenAPI documents declares a securitySchemes block or a security requirement\n    (derive-authentication.py therefore produced nothing), so this profile is read from the provider's own\n    documents. The primary model is payment in place of authentication: no account, no key, no OAuth — an\n    unpaid\
  \ call to a paid route returns HTTP 402 with x402 requirements and the caller retries with a signed\n    USDC authorization in X-PAYMENT (v1) or PAYMENT-SIGNATURE (v2). A second, optional model is a card-bought\n    API key that unlocks the same routes over plain HTTPS. The MCP host states explicitly that it uses no OAuth\n    (a JSON 404 at /.well-known/oauth-protected-resource), and no OpenID/OAuth discovery document exists on any\n    host. Agent Planets issues a free per-planet api_key on claim for its own mutating calls.\nschemes:\n- name: x402 payment (primary)\n  type: x402-payment\n  in: header\n  parameter: X-PAYMENT (x402 v1) | PAYMENT-SIGNATURE (x402 v2)\n  applied_to: 'the 85 paid store routes (x-payment-info on each), the planets /survey, /odds and /api/accept, and the oracle /oracle'\n  description: >-\n    api-docs, verbatim: \"GET any paid path -> HTTP 402 + PAYMENT-REQUIRED header -> sign EIP-3009 USDC\n    authorization on Base (eip155:8453) -> retry with X-PAYMENT header.\
  \ No account, no API key.\" The 402\n    observed live on 2026-09-19 carried an x402Version 1 JSON body plus PAYMENT-REQUIRED and WWW-Authenticate\n    (MPP …) headers holding a base64 x402 v2 envelope, so both client generations are served. Rails: Base\n    USDC (asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, payTo 0xc91cE6291eDC0713ec753BAFBA002506ffb2b95c,\n    scheme exact) and Solana USDC (payTo 2147pBT4LxoszjvLeGRxyVzpRnMi986VH3FAoprSs8Ez). Settlement via the\n    Coinbase CDP facilitator; maxTimeoutSeconds 300.\n  flow:\n  - Request the paid route with no credential → 402 with requirements (price in atomic USDC, payTo, asset, network, maxTimeoutSeconds).\n  - Sign an EIP-3009 transferWithAuthorization (Base) or an SPL transfer (Solana) for exactly maxAmountRequired.\n  - Retry the identical request with X-PAYMENT or PAYMENT-SIGNATURE carrying the base64 payload → 200 with data.\n  mcp_variant: 'the same payload is passed as the x_payment argument of a tools/call after a first\
  \ call returns the requirements (initialize instructions, verbatim: \"settle and retry with the signed payment payload in the x_payment argument\")'\n  sources:\n  - https://store.agentexchange.work/api-docs\n  - live 402 on GET https://store.agentexchange.work/chain/gas?chain=base (2026-09-19)\n- name: Card-bought API key (optional)\n  type: apiKey\n  in: header\n  parameter: 'Authorization: Bearer ak_… or X-API-Key'\n  applied_to: every store SKU over plain HTTPS\n  description: >-\n    billing/catalog.json, verbatim: \"Buy an API key with a credit/debit card. The key unlocks every SKU over\n    plain HTTPS (send `Authorization: Bearer ak_...` or `X-API-Key`).\" Plans: $29/month all-access, $19 one-time\n    1,000-call pack, and a not-yet-purchasable $0.01/call metered plan; \"Fair-use rate limited.\" The key prefix\n    ak_ is the provider's own statement.\n  sources:\n  - https://store.agentexchange.work/billing/catalog.json\n  - https://store.agentexchange.work/.well-known/usd.json\n\
  - name: Agent Planets api_key\n  type: apiKey\n  in: body\n  parameter: api_key\n  applied_to: planets mutating calls (terraform, build, post_offer, accept_offer …) and the $0.05 POST /api/accept\n  description: 'Issued free on POST /api/claim (\"Requires a planet api_key (free via POST /api/claim)\" — planets x402 catalog). Identity for the claimed planet, not a paid credential.'\n  sources:\n  - https://planets.agentexchange.work/.well-known/x402\n  - https://planets.agentexchange.work/llms.txt\n- name: none (free surfaces)\n  type: none\n  applied_to: GET /score, /samples, /docs, /api-docs, /status, /health, /v1/models, /badge, /market/tasks, the Clearing House register/discover/bid routes, planets /pulse, /api/planets, /handshakes, oracle /oracle/info, and every discovery document\n  description: Anonymous. CORS Access-Control-Allow-Origin * observed.\nmcp:\n  endpoint: https://store.agentexchange.work/mcp\n  auth: none (initialize and tools/list anonymous); paid tools x402-gated per\
  \ call via x_payment\n  oauth_protected_resource: 404 — JSON body {\"error\":\"not_oauth_protected\", \"authentication\":{\"type\":\"none\",\"protocol\":\"x402\",\"network\":\"base\",\"asset\":\"USDC\"}}\n  dynamic_client_registration: not offered\nattribution_headers:\n  note: 'Optional, non-authenticating headers the /partners document defines for installed integrations: x-agent-store-client (stable integration name), x-agent-store-install-id (stored only as a one-way fingerprint after a paid call), x-agent-store-referrer (public referrer id). They identify an integration for attribution and never grant access.'\nabsent:\n- OAuth 2.0 / OIDC (no discovery document on any of six hosts; the MCP host says so explicitly)\n- mutual TLS\n- signed requests beyond the x402 payment payload\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/authentication/agentexchange-work-authentication.yml
summary_line: x402-payment/apiKey · 4 schemes
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- AI Visibility
- Generative Engine Optimization
- Crypto
- Blockchain
- On-Chain Data
- Web Search
- Prediction Markets
- DeFi
- Macroeconomics
- Public Procurement
- Marketplace
- Agent-Native
---
