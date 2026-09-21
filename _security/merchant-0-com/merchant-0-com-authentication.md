---
anonymous_access: false
api_key_in: []
api_specs:
- filename: merchant-0-com-openapi.json
  format: json
  label: Merchant-0 A2A Protocol Server API
  slug: merchant-0-a2a-protocol-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merchant-0-com/refs/heads/main/openapi/merchant-0-com-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Merchant 0 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merchant-0 declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Merchant-0
provider_slug: merchant-0-com
scheme_count: 0
schemes: []
slug: merchant-0-com-authentication
source_filename: merchant-0-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.merchant-0.com/openapi.json\nderived_from: openapi/merchant-0-com-openapi.json\ndocs:\n- https://merchant-0.com/.well-known/agent-card.json\n- https://merchant-0.com/.well-known/did.json\nsummary: >-\n  The OpenAPI declares NO securitySchemes and NO security requirements on any of its 95 operations, and\n  derive-authentication.py therefore produced no profile. Read against the contract's own descriptions and\n  the agent card, the real model is: buyer-facing routes are open — a caller asserts its identity by placing\n  its own did:web DID in the request body (buyer_did) and, at the sign step, an opaque buyer_signature whose\n  message and key the contract never defines; access is then shaped by reputation (a FLAGGED DID gets a 402\n  proof-of-work challenge answered with the X-PoW-Solution header) and by a semantic firewall (403\n  sentinel_blocked), not by credentials. Trial execution is authenticated by a trial_nonce\
  \ issued with the\n  grant. Operator routes take an undocumented sandbox_token as a query or body field — \"Body-field token (NOT\n  Bearer) per the established convention\" — and answer 401 {\"detail\":\"Unauthorized\"} without it. There are no\n  API keys, no OAuth, no OIDC, no mTLS and no bearer tokens anywhere. The provider's own identity is a did:web\n  DID with a published Ed25519 key.\nschemes_declared: []\nschemes_observed:\n- id: buyer-did-assertion\n  type: body-field identity assertion\n  field: buyer_did (also subscriber_did as a query parameter on delivery/referral reads)\n  format: 'did:web:<domain> (AP2NegotiateBody description: {\"buyer_did\":\"did:web:...\"})'\n  applies_to: [ap2_negotiate_alias_api_ap2_negotiate_post, submit_intent_api_ap2_intent_post, checkout_api_ucp_checkout_post, ap2_dispute_file_api_ap2_dispute_post, post_trial_grant_api_ap2_trial_grant_post, get_subscription_delivery_api_subscriptions_delivery_get, get_referral_code_api_subscription_referral_code_get]\n\
  \  verification: >-\n    Not described. Nothing in the contract says the server resolves the DID document or checks a signature at\n    negotiate time; what it describes is reputation scoring on the DID (Diplomat, FLAGGED state), ownership\n    matching (\"Buyer match enforced against the contract owner so rival agents cannot file disputes on other\n    agents' contracts\") and, for referral codes, \"auth = proven active subscription for the supplied DID\".\n  privacy: 'Never echoed back — every response carries buyer_did_hash (\"Rule #11\").'\n- id: buyer-signature\n  type: body-field signature (opaque)\n  field: buyer_signature\n  applies_to: [ap2_sign_alias_api_ap2_sign_post, sign_cart_api_ap2_sign__intent_id__post]\n  detail: '\"The buyer_signature length is logged -- never the signature material itself.\" The signed message, algorithm and key are not specified; the card calls it \"AP2 buyer_signature\" under authentication.methods.'\n- id: pow-challenge\n  type: HTTP 402 proof-of-work\
  \ challenge / response header\n  header: X-PoW-Solution\n  applies_to: [ap2_negotiate_alias_api_ap2_negotiate_post]\n  detail: 'Issued only to FLAGGED buyers; \"SHA-256 difficulty 4\" per GET /api/publicist/manifest security.pow_challenge. Retry the same request with the solution in the header.'\n- id: trial-nonce\n  type: body-field one-time credential\n  fields: [trial_id, trial_nonce]\n  applies_to: [post_trial_execute_api_ap2_trial_execute_post]\n  detail: '\"Public (authenticated by trial_nonce)\"; issued by post_trial_grant, one per DID, expires 24h.'\n- id: operator-sandbox-token\n  type: query/body-field token (operator only)\n  field: sandbox_token\n  applies_to: [get_trial_status_api_trial_status_get, get_discovery_registry_package_api_discovery_registry_package_get, list_scout_proposals_api_scout_proposals_get, get_advocate_disputes_api_advocate_disputes_get, get_settlement_records_api_settlement_records_get, get_outbound_targets_api_outbound_targets_get, post_settlement_confirm_api_settlement_confirm_post,\
  \ update_harvest_threshold_config_harvest_threshold_post, update_credit_limit_config_credit_limit_post, 'and the other operator control-plane writes (emergency, config, scout, sentinel, strategist, diplomat, advocate, outbound)']\n  observed: {url: 'GET https://api.merchant-0.com/api/discovery/registry-package', status: 401, body: '{\"detail\":\"Unauthorized\"}'}\n  detail: Not a buyer credential and never issued to third parties. Recorded because the contract publishes these routes in the public document.\n- id: x-payment-header\n  type: header (declared, undocumented)\n  header: X-Payment\n  applies_to: [check_inventory_alias_api_ucp_inventory_check_get]\n  detail: The x402 header name, declared optional on one read; an anonymous GET returned 200 with the catalog. No 402 PaymentRequirements was observed and no other route declares it.\n- id: wise-webhook-signature\n  type: inbound webhook signature verification (provider is the verifier)\n  header: X-Signature-SHA256\n  applies_to: [wise_webhook_receiver_api_webhooks_wise_post]\n\
  \  detail: '\"RSA-SHA256 signature verification against Wise''s PUBLISHED production public key (NO DB operations until this passes)\"; always-200 contract. Documents how the provider authenticates Wise, not how callers authenticate to the provider.'\nprovider_identity:\n  did: did:web:merchant-0.com\n  did_document: https://merchant-0.com/.well-known/did.json\n  verification_method: {id: 'did:web:merchant-0.com#key-1', type: Ed25519VerificationKey2020, publicKeyMultibase: z6MktCZfJjbzX4rGjqf8bz9zBmBehF5cyPeWiyDR5uZ6nSRc}\n  purposes: [authentication, assertionMethod]\n  note: The card's authentication.methods lists \"DID Web\" first. The proof capability returns a merchant_signature; the DID key above is the only published key a verifier could try against it.\noauth: {declared: false, discovery: {oauth_authorization_server: 404, openid_configuration: 404, oauth_protected_resource: 404}}\napi_keys: {declared: false, issued: false}\nmtls: {declared: false}\ngaps:\n- No securitySchemes in\
  \ the contract, so every tooling-derived auth profile (SDK generators, gateways, this pipeline's own derive script) reads the API as unauthenticated.\n- The signing scheme for buyer_signature is unspecified; an integrator cannot produce a valid signature from the published material.\n- Public write operations (negotiate, dispute, trial-grant, intent, checkout) accept any buyer_did with no proof of control described.\n- Operator routes are published in the same document as buyer routes with no security requirement marking them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merchant-0-com/refs/heads/main/authentication/merchant-0-com-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- AP2
- Universal Commerce Protocol
- Trade Intelligence
- Market Intelligence
- Supply Chain
- Southeast Asia
- Decentralized Identity
- agent-native
---
