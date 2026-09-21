---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: apimesh-xyz-openapi.yml
  format: yaml
  label: APIMesh Web Analysis APIs
  slug: apimesh-web-analysis-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimesh-xyz/refs/heads/main/openapi/apimesh-xyz-openapi.yml
auth_types:
- apiKey
- x402
- mpp
- none
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apimesh Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIMesh secures its APIs with apiKey, x402, mpp, and none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIMesh
provider_slug: apimesh-xyz
scheme_count: 4
schemes:
- description: 'Prepaid-credit API key bought at https://apimesh.xyz/signup (Stripe Checkout); sent as Authorization: Bearer <key>. Each paid call deducts credits atomically before execution (RETIRED.md); credits never expire and are non-refundable (Terms §4).'
  header: Authorization
  key_prefix: sk_live_
  name: apiKey
  purchase_url: https://apimesh.xyz/signup
  scheme: bearer
  sources:
  - agent card securitySchemes.apiKey
  - https://apimesh.xyz/llms-full.txt
  status: purchasable at /signup (200) but no priced endpoint answers since 2026-05-11
  type: http
- asset: USDC
  challenge: 'HTTP 402 with WWW-Authenticate: Payment carrying price, wallet and network; client signs a USDC transfer and retries with the X-PAYMENT header'
  discovery:
  - https://apimesh.xyz/.well-known/x402.json
  - https://apimesh.xyz/.well-known/x402
  facilitator: Coinbase CDP
  name: x402
  network: base-mainnet (eip155:8453)
  protocol: x402
  sources:
  - agent card securitySchemes.x402
  - https://github.com/mbeato/APIMesh#1-x402----crypto-micropayments-default
  type: payment
  version: '1'
- challenge: 'same HTTP 402 / WWW-Authenticate: Payment flow; cards and stablecoins via Stripe Machine Payments Protocol; discovery via OpenAPI x-mpp annotations (none present in the served specs) and per-API /.well-known/mpp'
  discovery:
  - https://apimesh.xyz/.well-known/mpp
  - https://agentsmd.apimesh.xyz/.well-known/mpp
  - https://stripesig.apimesh.xyz/.well-known/mpp
  name: mpp
  protocol: mpp
  sources:
  - agent card securitySchemes.mpp
  - MPP manifest payment_methods
  type: payment
  version: draft-ryan-httpauth-payment
- applies_to:
  - POST https://agentsmd.apimesh.xyz/normalize
  - POST https://stripesig.apimesh.xyz/check
  - GET https://apimesh.xyz/wallet/{address}
  - GET https://apimesh.xyz/wallet/{address}/history
  - GET /health on every host
  description: Anonymous; per-IP rate limits are the only gate.
  name: none
  sources:
  - live probes 2026-09-19
  - https://github.com/mbeato/APIMesh#wallet--spend-tracking-free-no-auth
  type: none
slug: apimesh-xyz-authentication
source_filename: apimesh-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://apimesh.xyz/.well-known/agent-card.json\ndocs:\n- https://github.com/mbeato/APIMesh#payment-methods\n- https://apimesh.xyz/llms-full.txt\n- https://apimesh.xyz/.well-known/mpp\n- https://apimesh.xyz/legal/terms\nderived_from: openapi/_original/apimesh-xyz-openapi.json\nnote: >-\n  Neither served OpenAPI declares a securityScheme (derive-authentication.py found none), so this\n  profile is read from the documents that do describe access: the agent card's securitySchemes\n  block, the MPP manifest's payment_methods, the README and llms-full.txt. The marketplace model\n  was \"pay, don't authenticate\": an anonymous request to a paid endpoint received HTTP 402 with a\n  WWW-Authenticate: Payment challenge and the client either paid per request (x402 USDC on Base,\n  or Stripe MPP) or presented a prepaid-credit Bearer key. The two endpoints that are live today\n  (agentsmd POST /normalize, stripesig POST /check) require\
  \ no credential at all — confirmed\n  2026-09-19 with anonymous 200/400 responses. The one authenticated write observed, PUT\n  /wallet/{address}/cap, returned 401 anonymously and its credential type is undocumented.\nsummary:\n  types: [apiKey, x402, mpp, none]\n  api_key_in: [header]\n  oauth2_flows: []\n  live_surface_auth: none\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  key_prefix: sk_live_\n  description: 'Prepaid-credit API key bought at https://apimesh.xyz/signup (Stripe Checkout); sent as Authorization: Bearer <key>. Each paid call deducts credits atomically before execution (RETIRED.md); credits never expire and are non-refundable (Terms §4).'\n  purchase_url: https://apimesh.xyz/signup\n  sources: [agent card securitySchemes.apiKey, https://apimesh.xyz/llms-full.txt]\n  status: 'purchasable at /signup (200) but no priced endpoint answers since 2026-05-11'\n- name: x402\n  type: payment\n  protocol: x402\n  version: '1'\n  network: base-mainnet\
  \ (eip155:8453)\n  asset: USDC\n  facilitator: Coinbase CDP\n  challenge: 'HTTP 402 with WWW-Authenticate: Payment carrying price, wallet and network; client signs a USDC transfer and retries with the X-PAYMENT header'\n  discovery: [https://apimesh.xyz/.well-known/x402.json, https://apimesh.xyz/.well-known/x402]\n  sources: [agent card securitySchemes.x402, https://github.com/mbeato/APIMesh#1-x402----crypto-micropayments-default]\n- name: mpp\n  type: payment\n  protocol: mpp\n  version: draft-ryan-httpauth-payment\n  challenge: 'same HTTP 402 / WWW-Authenticate: Payment flow; cards and stablecoins via Stripe Machine Payments Protocol; discovery via OpenAPI x-mpp annotations (none present in the served specs) and per-API /.well-known/mpp'\n  discovery: [https://apimesh.xyz/.well-known/mpp, https://agentsmd.apimesh.xyz/.well-known/mpp, https://stripesig.apimesh.xyz/.well-known/mpp]\n  sources: [agent card securitySchemes.mpp, MPP manifest payment_methods]\n- name: none\n  type: none\n\
  \  applies_to: ['POST https://agentsmd.apimesh.xyz/normalize', 'POST https://stripesig.apimesh.xyz/check', 'GET https://apimesh.xyz/wallet/{address}', 'GET https://apimesh.xyz/wallet/{address}/history', 'GET /health on every host']\n  description: Anonymous; per-IP rate limits are the only gate.\n  sources: [live probes 2026-09-19, https://github.com/mbeato/APIMesh#wallet--spend-tracking-free-no-auth]\nmcp:\n  handshake_auth: none\n  environment: 'WALLET_PRIVATE_KEY (optional, secret) — funds x402 payments made by the tools; free /preview tools ran without it'\n  source: mcp/apimesh-xyz-mcp.yml\noauth: false\nopenid_connect: false\ndiscovery_probes:\n- {url: https://apimesh.xyz/.well-known/oauth-authorization-server, status: 404}\n- {url: https://apimesh.xyz/.well-known/oauth-protected-resource, status: 404}\n- {url: https://apimesh.xyz/.well-known/openid-configuration, status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimesh-xyz/refs/heads/main/authentication/apimesh-xyz-authentication.yml
summary_line: apiKey/x402/mpp/none · 4 schemes
tags:
- Web Analysis
- SEO
- Web Security
- Email Verification
- Developer Tools
- Micropayments
- x402
- MCP
- agent-native
- Webhook
- AI Coding Agents
- Open-Source
---
