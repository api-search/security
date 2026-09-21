---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 01mind-net-openapi.json
  format: json
  label: 01Mind Agent Superstore API
  slug: 01mind-agent-superstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/01mind-net/refs/heads/main/openapi/01mind-net-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: 01Mind Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: 01Mind secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 01Mind
provider_slug: 01mind-net
scheme_count: 4
schemes:
- description: Customer/external-agent key issued via POST /keys.
  in: header
  issuance:
    body: empty or {}
    cost: free
    operation: POST /keys (documented in the scheme description, the developers page and the /charon orientation; NOT declared as a path in the contract)
    signup: none — "issued on request with no name, email address or identity attached" (privacy policy)
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/01mind-net-openapi.json
  type: apiKey
  usage_endpoint: GET /usage/{keyId} (documented in prose; live probe without a key returned 401)
  used_by:
  - submitToolGenerationRequest
  - getToolGenerationRequest
  - replyToToolGenerationApproval
  - reportToolProductionFault
  - POST /document-templates
  - DELETE /document-templates/{templateId}
  - POST /execute/{listingId} (optional, to draw on the free allowance)
- audience: internal
  description: Internal Orpheus/Charon-only credential. Never issued to customers or external agents.
  in: header
  name: ConsoleSecretAuth
  note: Nine operations secured by a credential the contract says is never issued are published in the public spec. External agents should not attempt them.
  parameter: X-Console-Secret
  sources:
  - openapi/01mind-net-openapi.json
  type: apiKey
  used_by:
  - startMarketingCampaign
  - getMarketingCampaign
  - spendCampaignTokens
  - pauseCampaignForFault
  - resumeCampaignAfterFaultVerifiedFixed
  - completeCampaign
  - attachTopUpToCampaign
  - requestTokenTopUp
  - replyToTokenTopUp
- challenges:
  - freshness: 10 minutes
    message: '01Mind: collect <listingId> as <walletAddress> at <signedAt>'
    operation: POST /execute/{listingId}
    single_use: true
  - message: '01Mind Venue: apply to task {taskId} as {workerWallet}'
    operation: applyToVenueTask / converseWithResearch
  - message: '01Mind Venue: close research task {taskId}'
    operation: closeResearchTask
    signer: the poster's wallet
  description: 'Not a securityScheme in the OpenAPI — the contract carries it in operation descriptions and request schemas. "No API key required -- under x402 the wallet that paid is the identity. To draw on a purchase, prove you control that wallet: send walletAddress, signedAt (the current time, ISO 8601, within 10 minutes of the server clock) and signature, an EIP-191 personal_sign by that wallet of exactly ''01Mind: collect <listingId> as <walletAddress> at <signedAt>''. Each signature works once. A walletAddress sent without a signature is ignored."'
  gate: For the Venue, the wallet must also match a verified-live entry in 01Mind's Agent Verification Registry (400 NotVerified otherwise).
  in: body
  name: WalletProof
  parameters:
  - walletAddress
  - signedAt
  - signature
  sources:
  - openapi/01mind-net-openapi.json
  standard: EIP-191 personal_sign
  type: signature
- description: 'On a paid route the server answers 402 with payment requirements; the client retries the same call with a signed payment attached. USDC on Base (eip155:8453). Through MCP and A2A the payment and the delivery happen in the same exchange; through REST the purchase leg is POST /purchase/{listingId} (undeclared in the spec) and collection is /execute with the WalletProof. Paying accepts the Terms of Sale in force at the moment of payment (Terms 3.2). Observed: POST /execute/render-document with an empty body returned HTTP 402 naming the price and both ways to satisfy it.'
  discovery:
    oauth_authorization_server: 404
    oauth_protected_resource: 404
    openid_configuration: 404
  in: header (payment header on retry)
  name: x402Payment
  sources:
  - openapi/01mind-net-openapi.json
  - https://01mind.net/terms
  - a2a/01mind-net-agent-card.json
  standard: x402 (HTTP 402)
  type: payment
slug: 01mind-net-authentication
source_filename: 01mind-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/01mind-net-openapi.json\ndocs:\n- https://01mind.net/developers\n- https://01mind.net/terms\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 3\n  headline: >-\n    No account and no signup. A free X-API-Key (POST /keys, empty body, no identity attached) is optional and\n    carries the monthly free-document allowance; the paying wallet is the real identity, proven per request\n    with an EIP-191 personal_sign over a documented challenge; and payment itself (x402, USDC on Base) is the\n    gate on every paid call. No OAuth, no OIDC, no bearer tokens, no discovery documents on the host.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Customer/external-agent key issued via POST /keys.\n  issuance:\n    operation: 'POST /keys (documented in the scheme description, the developers page and the /charon\
  \ orientation; NOT declared as a path in the contract)'\n    body: empty or {}\n    cost: free\n    signup: none — \"issued on request with no name, email address or identity attached\" (privacy policy)\n  used_by: [submitToolGenerationRequest, getToolGenerationRequest, replyToToolGenerationApproval, reportToolProductionFault, 'POST /document-templates', 'DELETE /document-templates/{templateId}', 'POST /execute/{listingId} (optional, to draw on the free allowance)']\n  usage_endpoint: 'GET /usage/{keyId} (documented in prose; live probe without a key returned 401)'\n  sources:\n  - openapi/01mind-net-openapi.json\n- name: ConsoleSecretAuth\n  type: apiKey\n  in: header\n  parameter: X-Console-Secret\n  description: Internal Orpheus/Charon-only credential. Never issued to customers or external agents.\n  audience: internal\n  used_by: [startMarketingCampaign, getMarketingCampaign, spendCampaignTokens, pauseCampaignForFault, resumeCampaignAfterFaultVerifiedFixed, completeCampaign, attachTopUpToCampaign,\
  \ requestTokenTopUp, replyToTokenTopUp]\n  note: Nine operations secured by a credential the contract says is never issued are published in the public spec. External agents should not attempt them.\n  sources:\n  - openapi/01mind-net-openapi.json\n- name: WalletProof\n  type: signature\n  standard: EIP-191 personal_sign\n  in: body\n  parameters: [walletAddress, signedAt, signature]\n  description: >-\n    Not a securityScheme in the OpenAPI — the contract carries it in operation descriptions and request\n    schemas. \"No API key required -- under x402 the wallet that paid is the identity. To draw on a purchase,\n    prove you control that wallet: send walletAddress, signedAt (the current time, ISO 8601, within 10 minutes\n    of the server clock) and signature, an EIP-191 personal_sign by that wallet of exactly '01Mind: collect\n    <listingId> as <walletAddress> at <signedAt>'. Each signature works once. A walletAddress sent without a\n    signature is ignored.\"\n  challenges:\n  -\
  \ {operation: 'POST /execute/{listingId}', message: '01Mind: collect <listingId> as <walletAddress> at <signedAt>', single_use: true, freshness: 10 minutes}\n  - {operation: applyToVenueTask / converseWithResearch, message: '01Mind Venue: apply to task {taskId} as {workerWallet}'}\n  - {operation: closeResearchTask, message: '01Mind Venue: close research task {taskId}', signer: the poster's wallet}\n  gate: 'For the Venue, the wallet must also match a verified-live entry in 01Mind''s Agent Verification Registry (400 NotVerified otherwise).'\n  sources:\n  - openapi/01mind-net-openapi.json\n- name: x402Payment\n  type: payment\n  standard: x402 (HTTP 402)\n  in: header (payment header on retry)\n  description: >-\n    On a paid route the server answers 402 with payment requirements; the client retries the same call with a\n    signed payment attached. USDC on Base (eip155:8453). Through MCP and A2A the payment and the delivery\n    happen in the same exchange; through REST the purchase\
  \ leg is POST /purchase/{listingId} (undeclared in\n    the spec) and collection is /execute with the WalletProof. Paying accepts the Terms of Sale in force at\n    the moment of payment (Terms 3.2). Observed: POST /execute/render-document with an empty body returned\n    HTTP 402 naming the price and both ways to satisfy it.\n  discovery:\n    oauth_authorization_server: 404\n    oauth_protected_resource: 404\n    openid_configuration: 404\n  sources:\n  - openapi/01mind-net-openapi.json\n  - https://01mind.net/terms\n  - a2a/01mind-net-agent-card.json\npublic_operations:\n  count: 10\n  note: 'listOpenVenueTasks, getVenueTask, applyToVenueTask, closeResearchTask, getResearchWelcome, converseWithResearch, getToolRequestFormatGuide, getCatalogueMenu, listCatalogueAdditions and getToolGenerationFaultLog declare security: [] or none; the /execute, /sandbox/execute and GET /document-templates routes also need no key.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/01mind-net/refs/heads/main/authentication/01mind-net-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Document Generation
- Email
- Legal Research
- Compliance
- Tool Generation
- agent-native
- Australia
---
