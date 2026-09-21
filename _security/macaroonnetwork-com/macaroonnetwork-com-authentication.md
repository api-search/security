---
anonymous_access: true
api_key_in: []
api_specs:
- filename: macaroonnetwork-com-openapi.json
  format: json
  label: Macaroon Network Agent Services API
  slug: agent-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macaroonnetwork-com/refs/heads/main/openapi/macaroonnetwork-com-openapi.json
auth_types:
- none
- x402-payment
description: 'Public discovery endpoints require no identity. Protected commercial resources use the x402 v2 payment protocol: the client receives HTTP 402 with payment requirements in PAYMENT-REQUIRED, authorises payment according to the advertised scheme, retries with PAYMENT-SIGNATURE and receives PAYMENT-RESPONSE. A verified payment "authorizes only the requested resource transaction. It does not create an account, OAuth session, bearer token, API key, or persistent identity." The payment proof "is not a bearer credential for anything beyond the single call it was issued for -- there is nothing to store, refresh, or revoke."'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Macaroonnetwork Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macaroon Network secures its APIs with none and x402-payment across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Macaroon Network
provider_slug: macaroonnetwork-com
scheme_count: 3
schemes:
- applies_to: GET /listings, /listings/search, /listings/{id}, /api/public/*, /api/router/resolve, /api/receipts/{id}, /.well-known/*, /llms.txt, /auth.md, /health, /a2a (JSON-RPC), both MCP servers (initialize, tools/list, free tools), GET /execute/{id} (price preflight)
  name: anonymous
  sources:
  - https://macaroonnetwork.com/auth.md
  - openapi/macaroonnetwork-com-openapi.json
  type: none
- applies_to: POST /execute/{capability_id} (72 per-capability operations) and paid MCP tool calls (macaroons_execute; macaroons_purchase over L402)
  challenge: HTTP 402; header PAYMENT-REQUIRED = base64 JSON {x402Version 2, resource, accepts[{scheme exact, network eip155:8453, amount, asset USDC 0x8335...2913, payTo, maxTimeoutSeconds 60, extra}], extensions.bazaar}; the same JSON is the response body
  name: x402-payment
  observed: POST https://api.macaroonnetwork.com/execute/vat-validate-v1 -> 402 with PAYMENT-REQUIRED on 2026-09-19
  optional_headers:
  - 'X-Macaroon-Payment-Rail: x402'
  - 'X-Macaroon-X402-Network: base'
  proof: header PAYMENT-SIGNATURE = base64 signed payment payload from an x402 v2-compatible wallet (Coinbase CDP or self-managed)
  protocol: x402
  receipt: header PAYMENT-RESPONSE on the successful paid response; GET /api/receipts/{receipt_id} afterwards
  settlement: exact USDC on Base mainnet, predicate-gated (funds held, settled only if the acceptance predicate passes; failed predicate refunds automatically)
  sources:
  - https://macaroonnetwork.com/auth.md
  - openapi/macaroonnetwork-com-openapi.json (402 responses + x-payment-info)
  - https://macaroonnetwork.com/listings/vat-validate-v1
  type: payment
  version: v2
- description: An agent may optionally send a self-assigned X-Macaroon-Agent-Id header purely to scope its own free-tier quota -- this is never an identity or trust credential. Listing free_tier objects call it "self_declared_agent_id_until_account_auth_ships".
  name: X-Macaroon-Agent-Id
  purpose: quota scoping only
  sources:
  - https://macaroonnetwork.com/auth.md
  - https://api.macaroonnetwork.com/.well-known/ai-catalog.json
  type: header
slug: macaroonnetwork-com-authentication
source_filename: macaroonnetwork-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://macaroonnetwork.com/auth.md\nderived_from: openapi/macaroonnetwork-com-openapi.json\ndocs:\n- https://macaroonnetwork.com/auth.md\n- https://api.macaroonnetwork.com/.well-known/oauth-protected-resource\n- https://macaroonnetwork.com/listings/vat-validate-v1\n- https://macaroonnetwork.com/bible-api\nsummary:\n  types: [none, x402-payment]\n  api_key_in: []\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\n  identity_types_supported: [anonymous]\n  note: >-\n    The OpenAPI declares no securitySchemes and no security[] on any of its 120 operations, and that is\n    accurate rather than an omission: auth.md states \"Macaroon Network does not use OAuth registration, user\n    accounts, API keys, or bearer credentials for its public pay-per-call services.\" The mechanical\n    derive-authentication.py pass therefore produced no profile; this file is the documented model.\ndescription: >-\n  Public discovery endpoints\
  \ require no identity. Protected commercial resources use the x402 v2 payment\n  protocol: the client receives HTTP 402 with payment requirements in PAYMENT-REQUIRED, authorises payment\n  according to the advertised scheme, retries with PAYMENT-SIGNATURE and receives PAYMENT-RESPONSE. A verified\n  payment \"authorizes only the requested resource transaction. It does not create an account, OAuth session,\n  bearer token, API key, or persistent identity.\" The payment proof \"is not a bearer credential for anything\n  beyond the single call it was issued for -- there is nothing to store, refresh, or revoke.\"\nschemes:\n- name: anonymous\n  type: none\n  applies_to: GET /listings, /listings/search, /listings/{id}, /api/public/*, /api/router/resolve, /api/receipts/{id}, /.well-known/*, /llms.txt, /auth.md, /health, /a2a (JSON-RPC), both MCP servers (initialize, tools/list, free tools), GET /execute/{id} (price preflight)\n  sources: [https://macaroonnetwork.com/auth.md, openapi/macaroonnetwork-com-openapi.json]\n\
  - name: x402-payment\n  type: payment\n  protocol: x402\n  version: v2\n  applies_to: POST /execute/{capability_id} (72 per-capability operations) and paid MCP tool calls (macaroons_execute; macaroons_purchase over L402)\n  challenge: 'HTTP 402; header PAYMENT-REQUIRED = base64 JSON {x402Version 2, resource, accepts[{scheme exact, network eip155:8453, amount, asset USDC 0x8335...2913, payTo, maxTimeoutSeconds 60, extra}], extensions.bazaar}; the same JSON is the response body'\n  proof: 'header PAYMENT-SIGNATURE = base64 signed payment payload from an x402 v2-compatible wallet (Coinbase CDP or self-managed)'\n  receipt: 'header PAYMENT-RESPONSE on the successful paid response; GET /api/receipts/{receipt_id} afterwards'\n  optional_headers: ['X-Macaroon-Payment-Rail: x402', 'X-Macaroon-X402-Network: base']\n  settlement: exact USDC on Base mainnet, predicate-gated (funds held, settled only if the acceptance predicate passes; failed predicate refunds automatically)\n  observed: 'POST https://api.macaroonnetwork.com/execute/vat-validate-v1\
  \ -> 402 with PAYMENT-REQUIRED on 2026-09-19'\n  sources: [https://macaroonnetwork.com/auth.md, openapi/macaroonnetwork-com-openapi.json (402 responses + x-payment-info), https://macaroonnetwork.com/listings/vat-validate-v1]\n- name: X-Macaroon-Agent-Id\n  type: header\n  purpose: quota scoping only\n  description: 'An agent may optionally send a self-assigned X-Macaroon-Agent-Id header purely to scope its own free-tier quota -- this is never an identity or trust credential. Listing free_tier objects call it \"self_declared_agent_id_until_account_auth_ships\".'\n  sources: [https://macaroonnetwork.com/auth.md, https://api.macaroonnetwork.com/.well-known/ai-catalog.json]\noauth:\n  implemented: false\n  protected_resource_metadata:\n    url: https://api.macaroonnetwork.com/.well-known/oauth-protected-resource\n    also_on: [https://macaroonnetwork.com/.well-known/oauth-protected-resource, https://www.macaroonnetwork.com/.well-known/oauth-protected-resource]\n    resource: https://api.macaroonnetwork.com\n\
  \    resource_name: Macaroon Network API\n    resource_documentation: https://macaroonnetwork.com/auth.md\n    bearer_methods_supported: []\n    authorization_servers: []\n    note: 'auth.md: published \"for machine-readable resource discovery, but it intentionally advertises no authorization server.\" /.well-known/oauth-authorization-server and /.well-known/openid-configuration 404 on every host; no dynamic client registration.'\ncredentialed_human_surfaces:\n- name: Faith Evidence Pro\n  url: https://macaroonnetwork.com/bible-api\n  note: PayPal subscription ($19/month or $190/year) giving \"authenticated REST access to all eleven evidence operations\" with \"key recovery\". The key scheme (header name, issuance) is not documented publicly; not modelled here beyond this note.\n- name: Logistics Compliance Pro\n  url: https://macaroonnetwork.com/logistics-pro\n  note: 'PayPal subscription (£39/month); access is a private lookup link emailed on payment — \"No password, no separate account.\"\
  '\nmcp_auth:\n  router: none (initialize and tools/list anonymous; paid tools return the x402 challenge)\n  bible_evidence: none (free read-only tools; \"no API key required for the bounded tools\")\na2a_auth:\n  note: The agent card declares no securitySchemes; POST /a2a answered JSON-RPC anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macaroonnetwork-com/refs/heads/main/authentication/macaroonnetwork-com-authentication.yml
summary_line: none/x402-payment · 3 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Data Marketplace
- Compliance
- Sanctions Screening
- Company Data
- Scientific Computing
- Bible
- United Kingdom
- agent-native
---
