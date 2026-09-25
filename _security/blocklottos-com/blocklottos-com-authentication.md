---
anonymous_access: true
api_key_in: []
api_specs:
- filename: blocklottos-com-openapi.yml
  format: yaml
  label: Block Lottos API
  slug: block-lottos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blocklottos-com/refs/heads/main/openapi/blocklottos-com-openapi.yml
auth_types:
- none
- http-bearer
- wallet-signature
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Blocklottos Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Block Lottos secures its APIs with none, http-bearer, and wallet-signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Block Lottos
provider_slug: blocklottos-com
scheme_count: 4
schemes:
- applies_to: all GET operations, buildLotteryTicketTx, submitAd/activate quote and pay steps, getBaseAgentCapabilities, prepareBaseAgentPurchase, confirmBaseTicketPurchase
  name: public
  rate_limited: per IP (see rate-limits/)
  sources:
  - openapi/blocklottos-com-openapi.yml
  - https://blocklottos.com/api-docs
  type: none
- applies_to: getOrCreateUnifiedAffiliateProfile only - payout-wallet changes and private balance/payout-history reads
  bearerFormat: blm_ + 64 hex chars
  declared_as: an optional header PARAMETER on the operation, not a securityScheme - the contract therefore reports no security at all to tooling
  in: header
  issuance: Returned ONCE when a new affiliate profile is created (or rotated) after a successful ownership proof; "Store the one-time management_token securely".
  name: managementToken
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/blocklottos-com-openapi.yml
  - https://blocklottos.com/api-docs#agent-referral
  - https://blocklottos.com/llms.txt
  type: http
- applies_to: affiliate enrollment and management-token recovery
  cost: 0 USDC, no on-chain transaction
  flow:
  - POST /api/lottery/agent-referral {"action":"challenge","primary_chain":"evm","connected_wallet":"0x..."}
  - sign the exact returned message with the EVM identity wallet (EIP-191 personal_sign, 65-byte hex); the spec also accepts a Solana Ed25519 64-byte hex signature
  - resubmit with challenge_id (48 hex) + signature
  name: walletOwnershipChallenge
  sources:
  - openapi/blocklottos-com-openapi.yml
  - https://blocklottos.com/agents.txt
  type: wallet-signature
- name: onChainSignature
  note: 'Not API authentication, but the actual authorization for money: the API returns unsigned transactions and the wallet owner signs/broadcasts with eth_sendTransaction; "The Block Lottos server never receives private keys or seed phrases, never signs wallet transactions, and never broadcasts them." (llms.txt)'
  type: wallet-signature
slug: blocklottos-com-authentication
source_filename: blocklottos-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: 'openapi/blocklottos-com-openapi.yml (no securitySchemes; POST /api/lottery/agent-referral declares an optional\n  Authorization header parameter with pattern ^Bearer blm_[0-9a-f]{64}$), https://blocklottos.com/api-docs (#ads-overview\n  \"No API key required\", #lottery-overview \"Authentication: None required, all read endpoints are public\", #agent-referral\n  challenge/sign flow), /.well-known/ai-plugin.json auth.type none, /.well-known/agent.json trust.no_api_key_for_read_endpoints,\n  live CORS allow-headers 2026-09-19.'\ndocs: https://blocklottos.com/api-docs#agent-referral\nsummary:\n  types:\n  - none\n  - http-bearer\n  - wallet-signature\n  api_key_in: []\n  oauth2_flows: []\n  default: none - every read endpoint and every unsigned-transaction builder is public and key-less; access control\n    for money lives in the caller's wallet, not in the API.\nschemes:\n- name: public\n  type: none\n  applies_to: all GET operations,\
  \ buildLotteryTicketTx, submitAd/activate quote and pay steps, getBaseAgentCapabilities,\n    prepareBaseAgentPurchase, confirmBaseTicketPurchase\n  rate_limited: per IP (see rate-limits/)\n  sources:\n  - openapi/blocklottos-com-openapi.yml\n  - https://blocklottos.com/api-docs\n- name: managementToken\n  type: http\n  scheme: bearer\n  bearerFormat: blm_ + 64 hex chars\n  in: header\n  parameter: Authorization\n  applies_to: getOrCreateUnifiedAffiliateProfile only - payout-wallet changes and private balance/payout-history\n    reads\n  issuance: Returned ONCE when a new affiliate profile is created (or rotated) after a successful ownership proof;\n    \"Store the one-time management_token securely\".\n  declared_as: an optional header PARAMETER on the operation, not a securityScheme - the contract therefore reports\n    no security at all to tooling\n  sources:\n  - openapi/blocklottos-com-openapi.yml\n  - https://blocklottos.com/api-docs#agent-referral\n  - https://blocklottos.com/llms.txt\n\
  - name: walletOwnershipChallenge\n  type: wallet-signature\n  flow:\n  - POST /api/lottery/agent-referral {\"action\":\"challenge\",\"primary_chain\":\"evm\",\"connected_wallet\":\"0x...\"}\n  - sign the exact returned message with the EVM identity wallet (EIP-191 personal_sign, 65-byte hex); the spec\n    also accepts a Solana Ed25519 64-byte hex signature\n  - resubmit with challenge_id (48 hex) + signature\n  applies_to: affiliate enrollment and management-token recovery\n  cost: 0 USDC, no on-chain transaction\n  sources:\n  - openapi/blocklottos-com-openapi.yml\n  - https://blocklottos.com/agents.txt\n- name: onChainSignature\n  type: wallet-signature\n  note: 'Not API authentication, but the actual authorization for money: the API returns unsigned transactions and\n    the wallet owner signs/broadcasts with eth_sendTransaction; \"The Block Lottos server never receives private\n    keys or seed phrases, never signs wallet transactions, and never broadcasts them.\" (llms.txt)'\nidentification_headers:\n\
  - name: X-BlockLottos-Agent\n  required: false\n  purpose: optional agent identifier used in the docs curl examples; also carried as agent_id in bodies\n- name: X-BlockLottos-Intent\n  required: false\n  purpose: listed in Access-Control-Allow-Headers on the agent endpoints; undocumented\n- name: Idempotency-Key\n  required: false\n  purpose: listed in Access-Control-Allow-Headers on agent-purchase and agent-referral; the documented mechanism\n    is the idempotency_key body field (see conventions/)\ngaps:\n- No securitySchemes block, so the Bearer requirement is invisible to generated clients.\n- No scopes, no OAuth, no API-key issuance - nothing to record in scopes/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blocklottos-com/refs/heads/main/authentication/blocklottos-com-authentication.yml
summary_line: none/http-bearer/wallet-signature · 4 schemes
tags:
- Company
- Lottery
- Blockchain
- Web3
- Gaming
- Cryptocurrency
- Advertising
- Affiliate Marketing
- AI Agents
- Base
- Polygon
- USDC
- Smart Contracts
- A2A
---
