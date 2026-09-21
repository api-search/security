---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: babyblueviper-com-openapi.yml
  format: yaml
  label: invinoveritas API
  slug: invinoveritas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/openapi/babyblueviper-com-openapi.yml
auth_types:
- http-bearer
- l402
- x402
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Babyblueviper Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: invinoveritas secures its APIs with http-bearer, l402, x402, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: invinoveritas
provider_slug: babyblueviper-com
scheme_count: 4
schemes:
- applies_to: every paid REST endpoint and every paid MCP tool call; also account endpoints (/balance takes api_key as a query parameter instead)
  header: 'Authorization: Bearer <api_key>'
  key_prefix: ivv_
  name: bearer
  observed: 'POST /memory/store without credentials -> 401 {"detail":"Missing or invalid Bearer token (or send X-Payment-Scheme: x402 for USDC payment)"}'
  obtain: 'POST https://api.babyblueviper.com/register {"label": "my-agent"} (free, instant, no wallet)'
  scheme: bearer
  sources:
  - agent card securitySchemes.bearer
  - https://api.babyblueviper.com/guide
  - live 402 body "recommended_path"
  type: http
- applies_to: pay-per-call without a registered account (Lightning)
  challenge: 'HTTP 402 with WWW-Authenticate: L402 token="<hex>", invoice="<bolt11>" and Retry-After: 15'
  format: L402 <payment_hash>:<preimage>
  in: header
  name: l402
  parameter: Authorization
  sources:
  - agent card securitySchemes.l402
  - llms.txt "Payment methods"
  - live POST /reason and POST /review 402 responses
  type: apiKey
- catalog: https://api.babyblueviper.com/discovery/x402 (x402Version 2, 20 priced resources) and x-payment-info on 20 OpenAPI operations
  challenge: 'HTTP 402 with x-payment-scheme: x402, a base64 payment-required header (x402Version 2, accepts[] on eip155:8453 USDC) and the same JSON in the body'
  in: header
  name: x402
  network: eip155:8453 (Base), USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913; XRP Ledger also named in llms.txt/README
  opt_in_header: 'X-Payment-Scheme: x402'
  parameter: X-PAYMENT
  sources:
  - agent card securitySchemes.x402
  - OpenAPI info.x-guidance
  - live GET /regime and GET /signals/full 402 responses
  type: apiKey
- client_id_metadata_document_supported: true
  flows:
  - authorizationUrl: https://api.babyblueviper.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    refresh: true
    scopes:
      mcp: Access the invinoveritas MCP server
    tokenUrl: https://api.babyblueviper.com/oauth/token
  metadata: https://api.babyblueviper.com/.well-known/oauth-authorization-server
  name: oauth2
  note: No jwks_uri is published and no OIDC. Scopes are documented in scopes/babyblueviper-com-scopes.yml.
  protected_resource_metadata: https://api.babyblueviper.com/.well-known/oauth-protected-resource
  registration_endpoint: https://api.babyblueviper.com/oauth/register
  resource: https://api.babyblueviper.com/mcp
  sources:
  - RFC 8414 metadata
  - RFC 9728 metadata
  - MCP server card ("advertises OAuth2.1" per the provider roadmap)
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: babyblueviper-com-authentication
source_filename: babyblueviper-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs:\n- https://api.babyblueviper.com/guide\n- https://api.babyblueviper.com/wallet-onboarding\n- https://api.babyblueviper.com/llms.txt\n- https://api.babyblueviper.com/.well-known/oauth-authorization-server\n- https://api.babyblueviper.com/.well-known/agent-card.json\nsource: >-\n  The OpenAPI (openapi/babyblueviper-com-openapi.yml) declares NO components.securitySchemes — 167 of 187\n  operations carry security: [] and the paid ones carry an x-payment-info block instead of a scheme — so\n  derive-authentication.py produced nothing. This profile is written from the provider's payment guide,\n  wallet-onboarding page, llms.txt, the RFC 8414/9728 metadata, the agent card's securitySchemes block and\n  live 402/401 responses observed on 2026-09-19.\nsummary:\n  types: [http-bearer, l402, x402, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  default: Bearer api_key (free registration; the provider's recommended\
  \ path for agents)\n  note: >-\n    Four ways in. (1) Bearer: POST /register (no payment, no wallet) returns an api_key prefixed ivv_ ; send\n    Authorization: Bearer <api_key>; the first few paid calls are free (\"first 5 calls FREE\" in the live 402\n    body; \"free_calls_remaining\" in review responses), after which the balance must be funded via Lightning\n    top-up, x402 USDC or card. (2) L402: an unauthenticated POST to a paid endpoint returns 402 with\n    WWW-Authenticate: L402 token=\"...\", invoice=\"lnbc...\" — pay the bolt11 invoice and retry with\n    Authorization: L402 <payment_hash>:<preimage>. (3) x402: send X-Payment-Scheme: x402 (or hit an\n    x402-priced GET such as /regime) to receive a 402 whose payment-required header carries a base64 x402\n    v2 challenge (accepts[]: scheme exact, network eip155:8453, USDC asset, payTo, amount) and whose body is\n    the same JSON; retry with an X-PAYMENT header. (4) OAuth 2.1 for the MCP resource: RFC 8414 metadata at\n  \
  \  /.well-known/oauth-authorization-server (authorization_code + refresh_token, PKCE S256, dynamic client\n    registration, scope mcp). No OpenID Connect (the openid-configuration path says so explicitly).\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  key_prefix: ivv_\n  obtain: 'POST https://api.babyblueviper.com/register {\"label\": \"my-agent\"} (free, instant, no wallet)'\n  header: 'Authorization: Bearer <api_key>'\n  applies_to: every paid REST endpoint and every paid MCP tool call; also account endpoints (/balance takes api_key as a query parameter instead)\n  sources: [agent card securitySchemes.bearer, https://api.babyblueviper.com/guide, live 402 body \"recommended_path\"]\n  observed: 'POST /memory/store without credentials -> 401 {\"detail\":\"Missing or invalid Bearer token (or send X-Payment-Scheme: x402 for USDC payment)\"}'\n- name: l402\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'L402 <payment_hash>:<preimage>'\n  challenge: 'HTTP\
  \ 402 with WWW-Authenticate: L402 token=\"<hex>\", invoice=\"<bolt11>\" and Retry-After: 15'\n  applies_to: pay-per-call without a registered account (Lightning)\n  sources: [agent card securitySchemes.l402, llms.txt \"Payment methods\", live POST /reason and POST /review 402 responses]\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  opt_in_header: 'X-Payment-Scheme: x402'\n  challenge: 'HTTP 402 with x-payment-scheme: x402, a base64 payment-required header (x402Version 2, accepts[] on eip155:8453 USDC) and the same JSON in the body'\n  network: eip155:8453 (Base), USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913; XRP Ledger also named in llms.txt/README\n  catalog: https://api.babyblueviper.com/discovery/x402 (x402Version 2, 20 priced resources) and x-payment-info on 20 OpenAPI operations\n  sources: [agent card securitySchemes.x402, OpenAPI info.x-guidance, live GET /regime and GET /signals/full 402 responses]\n- name: oauth2\n  type: oauth2\n  resource: https://api.babyblueviper.com/mcp\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.babyblueviper.com/oauth/authorize\n    tokenUrl: https://api.babyblueviper.com/oauth/token\n    refresh: true\n    pkce: [S256]\n    scopes: {mcp: Access the invinoveritas MCP server}\n  registration_endpoint: https://api.babyblueviper.com/oauth/register\n  token_endpoint_auth_methods: [none, client_secret_post]\n  client_id_metadata_document_supported: true\n  metadata: https://api.babyblueviper.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://api.babyblueviper.com/.well-known/oauth-protected-resource\n  sources: [RFC 8414 metadata, RFC 9728 metadata, MCP server card (\"advertises OAuth2.1\" per the provider roadmap)]\n  note: No jwks_uri is published and no OIDC. Scopes are documented in scopes/babyblueviper-com-scopes.yml.\nfree_surface:\n  note: Operations marked security [] in the spec that are genuinely free with no credential — /verify-proof, /ledger*, /conformance*, /health,\
  \ /prices, /stats, /discovery/x402, /signals (teaser), the *-preview GETs, /offers/list, /messages/feed, the well-known documents and the docs pages.\nx-evidence:\n  fetched: '2026-09-19'\n  probes:\n  - {url: 'https://api.babyblueviper.com/reason', method: POST, status: 402, www_authenticate: L402, retry_after: 15}\n  - {url: 'https://api.babyblueviper.com/review', method: POST, status: 402, www_authenticate: L402, amount_sats: 260}\n  - {url: 'https://api.babyblueviper.com/regime', method: GET, status: 402, x_payment_scheme: x402}\n  - {url: 'https://api.babyblueviper.com/memory/store', method: POST, status: 401}\n  - {url: 'https://api.babyblueviper.com/balance', method: GET, status: 422, note: 'api_key query parameter required'}\n  - {url: 'https://api.babyblueviper.com/.well-known/oauth-authorization-server', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/authentication/babyblueviper-com-authentication.yml
summary_line: http-bearer/l402/x402/oauth2 · 4 schemes
tags:
- AI Agents
- Agent Verification
- Agent Governance
- MCP
- A2A
- Bitcoin Lightning
- x402
- Trading
- Cryptographic Proofs
- Agent Marketplace
---
