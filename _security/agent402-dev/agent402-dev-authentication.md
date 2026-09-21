---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agent402-dev-openapi.yml
  format: yaml
  label: Agent402 Direct x402 HTTP Resources
  slug: agent402-direct-x402-http-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent402-dev/refs/heads/main/openapi/agent402-dev-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agent402 Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: agent402.dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: agent402.dev
provider_slug: agent402-dev
scheme_count: 1
schemes:
- also_free:
  - /health
  - /metrics
  - /pmf/scorecard
  - /meta.json
  - /api/product
  - /openapi.json
  - /.well-known/x402
  - /llms.txt
  applies_to:
  - taskDayPlan
  - websitePreflight
  - verifiedUrlEvidence
  - siteReleaseAudit
  - auditX402
  - x402Health
  - downloadWayfarersDeck
  - downloadQrCampaignPack
  asset:
    contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    decimals: 6
    symbol: USDC
  challenge_status: 402
  client_requirement_verbatim: Use an x402-capable buyer client that validates the pinned terms and supplies PAYMENT-SIGNATURE. Plain curl is a 402 probe only and never pays.
  docs: https://agent402.dev/site-release-audit
  eip712_domain:
    name: USD Coin
    version: '2'
  free_routes:
  - siteReleaseAuditEligibility
  - siteReleaseAuditSample
  - siteReleaseAuditMethodology
  - siteReleaseAuditCaseStudy
  max_timeout_seconds: 300
  name: x402
  network: eip155:8453
  pay_to: '0xb0BbF890375B2ea1C2812887aE0331DD82eee92c'
  protocol: x402
  protocol_version: 2
  request_header: PAYMENT-SIGNATURE
  response_headers:
  - PAYMENT-REQUIRED
  - PAYMENT-RESPONSE
  scheme: exact
  type: payment
slug: agent402-dev-authentication
source_filename: agent402-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  openapi/agent402-dev-openapi.yml (x-payment-client-guidance, x-payment-info, 402 response descriptions,\n  info.x-guidance), https://agent402.dev/api/product (paymentClient, purchaseOptions, purchaseSafety),\n  https://agent402.dev/.well-known/x402 (accepts[]), the homepage \"Agent Payment\" / \"402 Retry Flow\" sections\n  and the /site-release-audit buyer-setup page, and live 402 challenges observed 2026-09-20 UTC.\ndocs: https://agent402.dev/site-release-audit\nchecked: '2026-09-19'\nsummary: >-\n  There is no authentication in the credential sense — no accounts, no sign-up, no API keys, no OAuth, no\n  sessions. Access to every paid resource is PAYMENT-AS-AUTHORIZATION under x402 v2: the first request gets\n  HTTP 402 with a PAYMENT-REQUIRED header naming the exact USDC amount on Base (eip155:8453) and the payee;\n  the client signs that authorization and repeats the identical request with a PAYMENT-SIGNATURE header;\n\
  \  the server verifies, delivers, and settles. Four support routes are free and anonymous. The OpenAPI\n  declares NO securitySchemes, so derive-authentication.py wrote nothing; this file is the searched\n  profile and overlays/ adds the scheme the contract omits.\nmodel: payment-as-authorization (x402 v2, exact scheme, USDC on Base)\naccounts: none — 'no account' (homepage and product page); 'buyer wallet required'\napi_keys: none\noauth2: none\nschemes:\n  - name: x402\n    type: payment\n    protocol: x402\n    protocol_version: 2\n    scheme: exact\n    network: eip155:8453\n    asset: {symbol: USDC, contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913', decimals: 6}\n    pay_to: '0xb0BbF890375B2ea1C2812887aE0331DD82eee92c'\n    request_header: PAYMENT-SIGNATURE\n    response_headers: [PAYMENT-REQUIRED, PAYMENT-RESPONSE]\n    challenge_status: 402\n    max_timeout_seconds: 300\n    eip712_domain: {name: USD Coin, version: '2'}   # accepts[].extra in the live challenge — the EIP-3009\
  \ transferWithAuthorization domain\n    applies_to: [\"taskDayPlan\", \"websitePreflight\", \"verifiedUrlEvidence\", \"siteReleaseAudit\", \"auditX402\", \"x402Health\", \"downloadWayfarersDeck\", \"downloadQrCampaignPack\"]\n    free_routes: [\"siteReleaseAuditEligibility\", \"siteReleaseAuditSample\", \"siteReleaseAuditMethodology\", \"siteReleaseAuditCaseStudy\"]\n    also_free: [/health, /metrics, /pmf/scorecard, /meta.json, /api/product, /openapi.json, /.well-known/x402, /llms.txt]\n    client_requirement_verbatim: 'Use an x402-capable buyer client that validates the pinned terms and supplies PAYMENT-SIGNATURE. Plain curl is a 402 probe only and never pays.'\n    docs: https://agent402.dev/site-release-audit\nbuyer_paths_published:\n  - {path: browser-wallet, detail: 'injected MetaMask or Coinbase Wallet on Base with >= 5 USDC; the page \"never receives or stores your private key\"; one signed attempt, no automatic retry', url: https://agent402.dev/site-release-audit}\n  - {path:\
  \ x402-client, detail: 'any x402 v2 client that binds PAYMENT-SIGNATURE to this resource and preserves the eligibility-checked body', url: https://agent402.dev/site-release-audit}\n  - {path: node-recipe, detail: 'npm install --save-exact @payanagent/sdk@0.2.2 @x402/fetch@2.18.0 @x402/evm@2.18.0 viem@2.55.1; WALLET_KEY env var; run once', url: https://agent402.dev/site-release-audit}\n  - {path: payan-marketplace, detail: 'agents-only alternate route, offer kh70zbzh8m5awkegpvn7tc82798aed20 (priceCents 500) at https://payanagent.com/x402/<offerId>; the provider warns Payan \"challenges before seller input validation\"', url: https://agent402.dev/api/product}\nidentity_and_delegation:\n  agent_identity: none — no Web Bot Auth, no HTTP Message Signatures, no ERC-8004 reference; the paying wallet is the only identity\n  delegated_identity: none\n  dynamic_client_registration: not applicable (no clients to register)\n  rfc9728_protected_resource_metadata: absent (404)\nspec_gaps:\n  - 'components.securitySchemes\
  \ is absent and no operation carries security[], so a generated client sees an open API; the x-payment-client-guidance extension on siteReleaseAudit and x-payment-info on the eight paid operations are where the contract actually states the requirement.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent402-dev/refs/heads/main/authentication/agent402-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- x402
- Agentic Payments
- Agentic Commerce
- AI Agents
- A2A
- Technical SEO
- Website Audits
- URL Evidence
- Developer Tools
- Base
---
