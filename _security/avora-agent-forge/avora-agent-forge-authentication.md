---
api_key_in: []
api_specs:
- filename: avora-agent-forge-agent-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Agent API
  slug: avora-agent-forge-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-agent-api-openapi.yml
- filename: avora-agent-forge-public-evidence-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Public Evidence API
  slug: avora-agent-forge-public-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-public-evidence-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Avora Agent Forge Authentication
name_suffix: Authentication
oauth_flows: []
overview: AVORA Agent Forge secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AVORA Agent Forge
provider_slug: avora-agent-forge
scheme_count: 0
schemes: []
slug: avora-agent-forge-authentication
source_filename: avora-agent-forge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: >-\n  https://avora-agent-forge.netlify.app/llms.txt +\n  https://avora-agent-forge.netlify.app/agent-forge/pricing.json +\n  openapi/avora-agent-forge-commerce-openapi.json\ndocs: https://avora-agent-forge.netlify.app/ai/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  model: unauthenticated-public-with-onchain-settlement-gate\nschemes: []\nnotes: >-\n  Neither OpenAPI declares a components.securitySchemes block and neither declares a\n  top-level security requirement, so every documented operation is callable anonymously.\n  This is intentional rather than an omission: the provider states access is\n  unauthenticated and that paid tiers are gated by non-custodial, user-signed Solana Pay\n  (USDC) settlement verified on-chain instead of by API keys.\nauthorization:\n  model: proof-of-payment\n  mechanism: Solana Pay (USDC) on Solana mainnet\n  custody: non-custodial\n  wallet_approval_required: true\n \
  \ gate_operation: verifyPaymentAndDeliverEvidence\n  validated_fields:\n    - recipient\n    - USDC mint\n    - amount\n    - reference\n    - product\n    - subject hash\n    - campaign memo\n    - payment age\n  denial_status: 402\n  denial_meaning: Matching on-chain payment not found yet.\n  note: >-\n    The bearer of a paid artifact is whoever can present a matching on-chain settlement\n    reference plus orderId. There is no account, no key issuance, and no revocation\n    surface - the payment reference is the credential.\nresponse_integrity:\n  mechanism: Ed25519 JWS signed receipts\n  jwks: https://avora-agent-forge.netlify.app/.well-known/jwks.json\n  jwks_file: ../well-known/avora-agent-forge-jwks.json\n  operation: getReceiptVerificationKeys\n  note: >-\n    Public-sector assessments return an Ed25519 JWS receipt that any third party can verify\n    against the published JWKS without contacting the provider. This is response\n    authentication, not caller authentication.\n\
  gaps:\n  - No caller identity of any kind, so per-caller rate limiting, quota, and revocation are\n    not expressible.\n  - No API key or OAuth surface, so there is no scopes artifact to derive.\n  - No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource\n    (both 404), consistent with the no-auth model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/authentication/avora-agent-forge-authentication.yml
summary_line: none · 0 schemes
tags:
- Blockchain
- Crypto
- Solana
- Token Risk
- Due Diligence
- On-chain Evidence
- Fraud Intelligence
- AI Agents
- MCP
- A2A
- Signed Receipts
- Provenance
- Non-custodial Payments
- USDC
- Solana Pay
- Public-sector AI Interoperability
---
