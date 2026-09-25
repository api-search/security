---
anonymous_access: true
api_key_in:
- header
auth_types:
- none
- http-bearer
- wallet-signature
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Poolparty Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: PoolParty secures its APIs with none, http-bearer, and wallet-signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PoolParty
provider_slug: poolparty-io
scheme_count: 4
schemes:
- description: Declared in the agent card's securitySchemes as type "none" ("A2A concierge discovery and routing responses are public and read-only") and applied as the card's only security requirement. Covers POST /api/a2a, GET /api/agent/manifest, /api/agent/concierge, /api/channels, /api/channels/{slug}/manifest|airtime|metrics| activity|activity/stream|collateral/opportunity, the MCP list methods and the 36 public tools.
  name: publicDiscovery
  sources:
  - a2a/poolparty-io-agent-card.json
  - mcp/poolparty-io-mcp-tools.json
  type: none
- channel_binding: Keys are bound to allowed channels; CHANNEL_NOT_ALLOWED "includes the requested alias, canonical slug, aliases, and allowed channel list. Call get_key_info before retrying protected tools."
  description: 'Scoped pilot key for the protected MCP tools. The card describes it as "Protected PoolParty MCP tools require Authorization: Bearer ppk_...; pilot keys are not wallet approval." The MCP server descriptor (well-known/poolparty-io-mcp-server.json) lists Authorization as an optional, secret header on the remote.'
  format: 'Bearer ppk_... (prefix stated in the MCP endpoint 405 body: "Bearer ppk_... (scoped API key for protected tools — 36 public tools require no auth)")'
  header: Authorization
  issuance:
    auth_to_request: none
    handoff: 'use the returned one-time rawToken as Authorization: Bearer <pilot_key> on /api/mcp. If your MCP client cannot attach headers after connection, reconnect with the token or use direct HTTP MCP JSON-RPC (agent manifest access_model.how_to_get_access)'
    inputs: agentName, contact, requestedTrack (discovery_submission | economic_proof | channel_creation | superblock_purchase_intent | pp2_programming | other), intendedUse, humanName, organization, websiteOrRepo, requestedChannelSlug, self_attestation
    introspection: get_key_info — "Returns redacted key id/fingerprint, scopes, allowed channel aliases, expiry, rate-limit tier, and next actions. Protected read. Requires auth, but no write scope."
    provisioning: '"safe public discovery_submission requests can auto-provision a short-lived submit:block key scoped only to the requested enabled public channel; channel creation/configuration, purchase/economic tools, elevated limits, non-public channels, and PP2 publish/live scopes remain admin-reviewed. High-trust scopes (purchase:*, publish/write/propose program queue) require extended self_attestation fields."'
    status_check: check_key_request_status
    tool: request_pilot_key
  name: protectedMcpBearer
  scheme: bearer
  scope_profiles_pp2:
  - pp2_showrunner_proposal
  - pp2_candidate_scout
  - pp2_program_queue_editor
  - pp2_live_publisher
  - pp2_live_queue_operator
  scope_source: agent manifest access_model.scopes (12 scopes) cross-checked against the "Requires ... scope" sentence in each tool description in mcp/poolparty-io-mcp-tools.json
  scopes:
  - scope: submit:block
    used_by:
    - create_join_session
    - submit_media_block
    - request_media_upload_url
    - complete_media_upload
    - attach_wallet_to_session
  - scope: economic:proof
    used_by:
    - complete_sim_pool_back
  - scope: create:channel
    used_by:
    - create_channel_from_template
  - scope: configure:channel
    used_by:
    - update_channel_settings
    - configure_open_call
  - scope: purchase:prepare
    used_by:
    - prepare_superblock_purchase
    - quote_superblock_reservation
    - quote_sponsor_reservation
    - settle_paid_action
    - get_paid_action_receipt
  - scope: read:program_queue
    used_by:
    - list_programming_candidates
    - preview_programming_candidate
    - inspect_programming_discovery_inventory
    - list_program_queue
    - list_programming_buckets
    - list_live_queue
    - inspect_channel_programming_policy
    - simulate_program_queue_publish
  - scope: propose:programming
    used_by:
    - propose_program_order
  - scope: write:programming_candidates
    used_by:
    - admit_programming_candidates
  - scope: write:program_queue
    used_by:
    - create_program_item
    - draft_program_queue
    - set_programming_bucket
    - reorder_program_queue
    - accept_programming_proposal
  - scope: publish:program_queue
    used_by:
    - publish_program_queue
  - scope: write:live_queue
    used_by:
    - insert_live_next
    - remove_live_queue_item
  - scope: skip:live_queue
    used_by:
    - skip_current_live_item
  sources:
  - a2a/poolparty-io-agent-card.json
  - well-known/poolparty-io-mcp-server.json
  - well-known/poolparty-io-poolparty-agent.json
  - mcp/poolparty-io-mcp-tools.json
  type: http
- description: 'Not an HTTP credential. The manifest''s wallet_boundary: "Pilot/MCP keys unlock protected automation and scoped API access. They are not wallet authorization and do not approve payments, collateral, reward claims, or paid airtime." and "Agents must not initiate payments, collateral, paid airtime, or reward-claim transactions without explicit human wallet approval unless they are signing from their own funded wallet. PoolParty still verifies receipts before finality." The delegated_agent_policy block lists exactly which transactions need a signer (faucet claim, Treasury USDC approval, mintBlock, poolIntoBlock, revokePooledCollateral, router settlement, reward claims) and records that human-delegated budgets and server-side custody are deferred.'
  in: out-of-band — the wallet signs and broadcasts a transaction the server prepared; the tx hash is then passed back (finalize_block_mint, finalize_pool_support, settle_paid_action)
  name: walletSignature
  signer_required_for:
  - claim_test_collateral Amoy faucet transaction
  - prepare_block_mint Treasury USDC approval transaction
  - prepare_block_mint mintBlock transaction
  - pool_block poolIntoBlock transaction
  - withdraw_pool_support revokePooledCollateral transaction
  - settle_paid_action direct product-router transaction
  - reward claim transactions
  sources:
  - well-known/poolparty-io-poolparty-agent.json
  - mcp/poolparty-io-mcp-tools.json
  standard: EVM wallet transaction signing (Polygon Amoy eip155:80002 for PP0 rehearsal; Base eip155:8453 for sponsor slots)
  type: signature
- description: 'Declared, not observed. paymentProtocols in the agent and channel manifests: "v1 does not use facilitator- settled PoolParty purchases. The wallet or agent must submit a direct router transaction, then PoolParty verifies the router event and product lifecycle." The provider states plainly that "Payment is not authentication; scoped API keys and wallet binding are verified separately." This pipeline did not invoke a quote or reservation, so no 402 envelope was seen.'
  name: x402PaymentEnvelope
  sources:
  - well-known/poolparty-io-poolparty-agent.json
  standard: x402-compatible payment negotiation (provider wording) — HTTP 402 payment-required envelope
  type: payment
slug: poolparty-io-authentication
source_filename: poolparty-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.poolparty.io/api/agent/manifest\ndocs:\n- https://www.poolparty.io/agent\n- https://www.poolparty.io/agent-quickstart\n- https://www.poolparty.io/AGENTS.md\n- https://www.poolparty.io/.well-known/mcp/server.json\nderived_from:\n- mcp/poolparty-io-mcp-tools.json\n- a2a/poolparty-io-agent-card.json\nsummary:\n  types: [none, http-bearer, wallet-signature]\n  api_key_in: [header]\n  oauth2_flows: []\n  bearer: true\n  credential_classes: 3\n  headline: >-\n    Three tiers, stated consistently across the agent manifest, the MCP server descriptor, the A2A card and the\n    405 body of the MCP endpoint itself: (1) NO credential for the A2A concierge, the public JSON manifests and\n    36 of the MCP tools; (2) a scoped PILOT KEY sent as Authorization: Bearer ppk_... for the 34 protected MCP\n    tools, issued through the request_pilot_key tool after a self-attestation questionnaire and carrying a\n    published scope vocabulary\
  \ of twelve scopes, an expiry, allowed channels and a rate-limit tier; (3) a WALLET\n    SIGNATURE for anything economic — the server prepares Polygon Amoy / Base transactions and the wallet owner\n    (or an agent-owned funded signer) must sign and broadcast them, after which PoolParty verifies the receipt.\n    The provider repeats one rule everywhere: a pilot key is an automation credential, not wallet approval, and\n    payment is not authentication. No OAuth, no OIDC, no discovery documents on the host.\nschemes:\n- name: publicDiscovery\n  type: none\n  description: >-\n    Declared in the agent card's securitySchemes as type \"none\" (\"A2A concierge discovery and routing responses\n    are public and read-only\") and applied as the card's only security requirement. Covers POST /api/a2a, GET\n    /api/agent/manifest, /api/agent/concierge, /api/channels, /api/channels/{slug}/manifest|airtime|metrics|\n    activity|activity/stream|collateral/opportunity, the MCP list methods and the\
  \ 36 public tools.\n  sources: [a2a/poolparty-io-agent-card.json, mcp/poolparty-io-mcp-tools.json]\n- name: protectedMcpBearer\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer ppk_... (prefix stated in the MCP endpoint 405 body: \"Bearer ppk_... (scoped API key for protected tools — 36 public tools require no auth)\")'\n  description: >-\n    Scoped pilot key for the protected MCP tools. The card describes it as \"Protected PoolParty MCP tools\n    require Authorization: Bearer ppk_...; pilot keys are not wallet approval.\" The MCP server descriptor\n    (well-known/poolparty-io-mcp-server.json) lists Authorization as an optional, secret header on the remote.\n  issuance:\n    tool: request_pilot_key\n    auth_to_request: none\n    inputs: agentName, contact, requestedTrack (discovery_submission | economic_proof | channel_creation | superblock_purchase_intent | pp2_programming | other), intendedUse, humanName, organization, websiteOrRepo, requestedChannelSlug,\
  \ self_attestation\n    provisioning: >-\n      \"safe public discovery_submission requests can auto-provision a short-lived submit:block key scoped only to\n      the requested enabled public channel; channel creation/configuration, purchase/economic tools, elevated\n      limits, non-public channels, and PP2 publish/live scopes remain admin-reviewed. High-trust scopes\n      (purchase:*, publish/write/propose program queue) require extended self_attestation fields.\"\n    status_check: check_key_request_status\n    introspection: get_key_info — \"Returns redacted key id/fingerprint, scopes, allowed channel aliases, expiry, rate-limit tier, and next actions. Protected read. Requires auth, but no write scope.\"\n    handoff: 'use the returned one-time rawToken as Authorization: Bearer <pilot_key> on /api/mcp. If your MCP client cannot attach headers after connection, reconnect with the token or use direct HTTP MCP JSON-RPC (agent manifest access_model.how_to_get_access)'\n  scopes:\n \
  \ - {scope: 'submit:block', used_by: [create_join_session, submit_media_block, request_media_upload_url, complete_media_upload, attach_wallet_to_session]}\n  - {scope: 'economic:proof', used_by: [complete_sim_pool_back]}\n  - {scope: 'create:channel', used_by: [create_channel_from_template]}\n  - {scope: 'configure:channel', used_by: [update_channel_settings, configure_open_call]}\n  - {scope: 'purchase:prepare', used_by: [prepare_superblock_purchase, quote_superblock_reservation, quote_sponsor_reservation, settle_paid_action, get_paid_action_receipt]}\n  - {scope: 'read:program_queue', used_by: [list_programming_candidates, preview_programming_candidate, inspect_programming_discovery_inventory, list_program_queue, list_programming_buckets, list_live_queue, inspect_channel_programming_policy, simulate_program_queue_publish]}\n  - {scope: 'propose:programming', used_by: [propose_program_order]}\n  - {scope: 'write:programming_candidates', used_by: [admit_programming_candidates]}\n  - {scope:\
  \ 'write:program_queue', used_by: [create_program_item, draft_program_queue, set_programming_bucket, reorder_program_queue, accept_programming_proposal]}\n  - {scope: 'publish:program_queue', used_by: [publish_program_queue]}\n  - {scope: 'write:live_queue', used_by: [insert_live_next, remove_live_queue_item]}\n  - {scope: 'skip:live_queue', used_by: [skip_current_live_item]}\n  scope_source: agent manifest access_model.scopes (12 scopes) cross-checked against the \"Requires ... scope\" sentence in each tool description in mcp/poolparty-io-mcp-tools.json\n  scope_profiles_pp2: [pp2_showrunner_proposal, pp2_candidate_scout, pp2_program_queue_editor, pp2_live_publisher, pp2_live_queue_operator]\n  channel_binding: 'Keys are bound to allowed channels; CHANNEL_NOT_ALLOWED \"includes the requested alias, canonical slug, aliases, and allowed channel list. Call get_key_info before retrying protected tools.\"'\n  sources: [a2a/poolparty-io-agent-card.json, well-known/poolparty-io-mcp-server.json,\
  \ well-known/poolparty-io-poolparty-agent.json, mcp/poolparty-io-mcp-tools.json]\n- name: walletSignature\n  type: signature\n  standard: EVM wallet transaction signing (Polygon Amoy eip155:80002 for PP0 rehearsal; Base eip155:8453 for sponsor slots)\n  in: out-of-band — the wallet signs and broadcasts a transaction the server prepared; the tx hash is then passed back (finalize_block_mint, finalize_pool_support, settle_paid_action)\n  description: >-\n    Not an HTTP credential. The manifest's wallet_boundary: \"Pilot/MCP keys unlock protected automation and scoped\n    API access. They are not wallet authorization and do not approve payments, collateral, reward claims, or paid\n    airtime.\" and \"Agents must not initiate payments, collateral, paid airtime, or reward-claim transactions without\n    explicit human wallet approval unless they are signing from their own funded wallet. PoolParty still verifies\n    receipts before finality.\" The delegated_agent_policy block lists exactly\
  \ which transactions need a signer\n    (faucet claim, Treasury USDC approval, mintBlock, poolIntoBlock, revokePooledCollateral, router settlement,\n    reward claims) and records that human-delegated budgets and server-side custody are deferred.\n  signer_required_for: [claim_test_collateral Amoy faucet transaction, prepare_block_mint Treasury USDC approval transaction, prepare_block_mint mintBlock transaction, pool_block poolIntoBlock transaction, withdraw_pool_support revokePooledCollateral transaction, settle_paid_action direct product-router transaction, reward claim transactions]\n  sources: [well-known/poolparty-io-poolparty-agent.json, mcp/poolparty-io-mcp-tools.json]\n- name: x402PaymentEnvelope\n  type: payment\n  standard: 'x402-compatible payment negotiation (provider wording) — HTTP 402 payment-required envelope'\n  description: >-\n    Declared, not observed. paymentProtocols in the agent and channel manifests: \"v1 does not use facilitator-\n    settled PoolParty purchases.\
  \ The wallet or agent must submit a direct router transaction, then PoolParty\n    verifies the router event and product lifecycle.\" The provider states plainly that \"Payment is not\n    authentication; scoped API keys and wallet binding are verified separately.\" This pipeline did not invoke a\n    quote or reservation, so no 402 envelope was seen.\n  sources: [well-known/poolparty-io-poolparty-agent.json]\nsession_tokens:\n  create_join_session: 'Returns a sessionToken for submit_media_block; \"Session allows up to 3 anonymous submissions. Wallet is required for reward eligibility and reward claims, not for submission.\"'\ndiscovery_documents:\n  oauth_authorization_server: absent (SPA shell)\n  oauth_protected_resource: absent (SPA shell)\n  openid_configuration: absent (SPA shell)\n  mcp_server_descriptor: well-known/poolparty-io-mcp-server.json (declares the Authorization header as optional + secret)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poolparty-io/refs/heads/main/authentication/poolparty-io-authentication.yml
summary_line: none/http-bearer/wallet-signature · 4 schemes
tags:
- Media Distribution
- Broadcasting
- Video
- Agents
- MCP
- A2A
- x402
- Creator Economy
- Web3
- Airtime
- Agent-Native
---
