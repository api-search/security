---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agenthealthmonitor-xyz-openapi.yml
  format: yaml
  label: Agent Health Monitor API
  slug: agent-health-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/openapi/agenthealthmonitor-xyz-openapi.yml
- filename: agenthealthmonitor-xyz-verify-openapi.yml
  format: yaml
  label: AHM Verify API
  slug: ahm-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/openapi/agenthealthmonitor-xyz-verify-openapi.yml
auth_types:
- apiKey
- x402-payment
- internal-key
- coupon
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Agenthealthmonitor Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Intensity Ltd secures its APIs with apiKey, x402-payment, internal-key, and coupon across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Digital Intensity Ltd
provider_slug: agenthealthmonitor-xyz
scheme_count: 4
schemes:
- applies_to: every paid operation as an alternative to x402 (the source lists the X-API-Key bypass paths); required on api_key_status_api_key_status_get and partner_usage_partners__partner_id__usage_get
  errors:
    '401': '{"detail":"X-API-Key header required"} / {"detail":"Invalid or expired API key"}'
    '429': '{"detail":"API key calls exhausted"}'
  header: 'X-API-Key: ahm_live_<secret>'
  in: header
  issuance: Stripe payment links on https://agenthealthmonitor.xyz/pay-by-card; after checkout the key is retrieved once at GET /stripe/key/{session_id} (retrieve_key_stripe_key__session_id__get). Also via the design-partner programme.
  key_format: ahm_live_ prefix (README, SDK examples, source); the docs quick-start shows ahm_sk_… — treat ahm_live_ as authoritative. Keys are credit-metered (Starter 100 / Pro 500 calls) or unlimited on the $99/month subscription; stored server-side and validated per request.
  name: ApiKeyAuth
  observed: GET https://agenthealthmonitor.xyz/api/key/status -> 401 {"detail":"X-API-Key header required"} (2026-09-19)
  parameter: X-API-Key
  rotation: Not documented. No revoke/rotate operation in the API.
  sources:
  - https://docs.agenthealthmonitor.xyz/#gs-api
  - README
  type: apiKey
- applies_to: the 15 payable resources in /.well-known/x402 (all 14 documented endpoints plus PUT /ahs/route/policy) and AHM Verify POST /v1/outputs
  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (EIP-712 domain name "USD Coin" version "2")
  facilitator: https://facilitator.payai.network
  flow: 1) call the endpoint; 2) receive 402 with body {} and PAYMENT-REQUIRED = base64 JSON {x402Version 2, error "Payment required", resource{url, description, mimeType}, accepts[{scheme, network, asset, amount, payTo, maxTimeoutSeconds, extra}], extensions.bazaar}; 3) sign an EIP-3009 transferWithAuthorization for accepts[0]; 4) resend with X-PAYMENT; the facilitator verifies and settles.
  identity: 'The payer wallet address becomes the caller identity for stateful routes (routing policy owner, batch limits) — "x402 callers: owner_id = lowercased payer wallet" in source.'
  in: header
  max_timeout_seconds: 300
  name: X402Payment
  network: eip155:8453 (Base mainnet)
  observed: GET /risk/0x0000000000000000000000000000000000000001 -> 402, accepts[0].amount 1000 (= $0.001); GET /ahs/route/policy -> 402 amount 10000; POST https://verify.agenthealthmonitor.xyz/v1/outputs -> 402 amount 500000 (2026-09-19)
  parameter: X-PAYMENT (request) / PAYMENT-REQUIRED (402 challenge response)
  pay_to:
    ahm_verify: '0x23A2e9Cd7F0a602A3FcFFaf8074113A9205726E5'
    main_api: '0xaD64EFCe9CfeE4d1D1701d9a0009CCa72B9ff000'
  scheme: exact
  sources:
  - https://agenthealthmonitor.xyz/.well-known/x402
  - live 402 on GET /risk/{address}, GET /ahs/route/policy, POST verify /v1/outputs
  type: x402
  version: 2
- applies_to:
  - security_activity_security_activity_get
  - trust_registry_trust_registry_get
  - internal_agent_profile_internal_agent_profile__address__get
  - trigger_acp_scan_acp_scan_trigger_post
  - acp_scan_status_acp_scan_status_get
  - trigger_olas_scan_olas_scan_trigger_post
  - olas_scan_status_olas_scan_status_get
  - trigger_arc_scan_arc_scan_trigger_post
  - arc_scan_status_arc_scan_status_get
  - trigger_celo_scan_celo_scan_trigger_post
  - celo_scan_status_celo_scan_status_get
  - trigger_erc8004_scan_erc8004_scan_trigger_post
  - erc8004_scan_status_erc8004_scan_status_get
  - erc8183_status_erc8183_status_get
  in: header
  name: InternalKey
  note: Operator-only; also bypasses x402 on paid routes (source). Not obtainable by customers.
  observed: GET /trust-registry -> 401 {"detail":"Unauthorized"}
  parameter: X-Internal-Key
  sources:
  - 'openapi operation descriptions (Admin tag: "Protected by X-Internal-Key header. Not accessible via x402 payment.")'
  type: apiKey
- applies_to:
  - validate_coupon_coupon_validate__code__get
  - coupon_risk_coupon_risk__code___address__get
  - coupon_health_coupon_health__code___address__get
  - coupon_optimize_coupon_optimize__code___address__get
  - coupon_retry_coupon_retry__code___address__get
  - coupon_protect_coupon_protect__code___address__get
  - coupon_alerts_coupon_alerts__code___address__get
  - coupon_premium_risk_coupon_risk_premium__code___address__get
  - coupon_counterparties_coupon_counterparties__code___address__get
  - coupon_network_map_coupon_network_map__code___address__get
  - coupon_wash_coupon_wash__code___address__get
  - coupon_ahs_coupon_ahs__code___address__get
  - coupon_report_card_coupon_report_card__code___address__get
  in: path
  name: CouponCode
  note: Partner-issued codes; rate-limited to 5 attempts per window on validation and access (source). A credential in the URL path, so it appears in logs and caches.
  parameter: '{code} in /coupon/{action}/{code}/{address}'
  sources:
  - 'openapi info.description: "partners can use coupon codes to access any paid endpoint without x402 payment"'
  type: path-token
slug: agenthealthmonitor-xyz-authentication
source_filename: agenthealthmonitor-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/agenthealthmonitor-xyz-openapi.yml and openapi/agenthealthmonitor-xyz-verify-openapi.yml (NEITHER declares\n  components.securitySchemes or security[] — derive-authentication.py produced nothing, so this profile is built from the\n  docs and live probes)\ndocs: https://docs.agenthealthmonitor.xyz/#gs-api\nadditional_docs:\n- https://docs.agenthealthmonitor.xyz/#integration\n- https://github.com/moonshot-cyber/agent-health-monitor#stripe-fiat--no-wallet-required\n- https://agenthealthmonitor.xyz/.well-known/x402\n- openapi info.description (Payment / Free preview / Coupon access paragraphs)\nsummary:\n  types:\n  - apiKey\n  - x402-payment\n  - internal-key\n  - coupon\n  http_schemes: []\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  credential_types:\n  - ahm_live_ API key (Stripe credit pack or subscription)\n  - x402 v2 payment proof (X-PAYMENT header) — USDC on eip155:8453\n\
  \  - X-Internal-Key (operator only)\n  - partner coupon code in the URL path\n  public_operations:\n  - api_info_api_info_get\n  - ecosystem_stats_api_ecosystem_stats_get\n  - leaderboard_api_leaderboard_get\n  - get_agent_public_api_agent__address__get\n  - endpoint_info_api_endpoint_info__slug__get\n  - retry_preview_retry_preview__address__get\n  - protection_preview_agent_protect_preview__address__get\n  - alert_status_alerts_status__address__get\n  - configure_alerts_alerts_configure_post\n  - unsubscribe_alerts_alerts_unsubscribe__address__delete\n  - up_up_get\n  - a2a_agent_card__well_known_agent_json_get\n  - x402_discovery__well_known_x402_get\n  - agent_registration__well_known_agent_registration_json_get\n  - create_spec_v1_specs_post (Verify)\n  - get_verdict_v1_verdicts__verdict_id__get (Verify)\n  - health_health_get (Verify)\n  discovery: None of RFC 9728 / RFC 8414 / OIDC. The only machine-readable auth discovery is the x402 402 challenge itself\n    (PAYMENT-REQUIRED\
  \ header) and /.well-known/x402.\n  dynamic_client_registration: false\n  delegated_identity: false\n  agent_onboarding: Fully autonomous via x402 — an agent with a funded Base wallet needs no account, key or human step; the\n    fiat path needs a human to pay via Stripe and paste the key.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - https://docs.agenthealthmonitor.xyz/#gs-api\n  - README\n  applies_to: every paid operation as an alternative to x402 (the source lists the X-API-Key bypass paths); required on api_key_status_api_key_status_get\n    and partner_usage_partners__partner_id__usage_get\n  header: 'X-API-Key: ahm_live_<secret>'\n  key_format: ahm_live_ prefix (README, SDK examples, source); the docs quick-start shows ahm_sk_… — treat ahm_live_ as authoritative.\n    Keys are credit-metered (Starter 100 / Pro 500 calls) or unlimited on the $99/month subscription; stored server-side and\n    validated per request.\n  issuance:\
  \ Stripe payment links on https://agenthealthmonitor.xyz/pay-by-card; after checkout the key is retrieved once at\n    GET /stripe/key/{session_id} (retrieve_key_stripe_key__session_id__get). Also via the design-partner programme.\n  rotation: Not documented. No revoke/rotate operation in the API.\n  errors:\n    '401': '{\"detail\":\"X-API-Key header required\"} / {\"detail\":\"Invalid or expired API key\"}'\n    '429': '{\"detail\":\"API key calls exhausted\"}'\n  observed: GET https://agenthealthmonitor.xyz/api/key/status -> 401 {\"detail\":\"X-API-Key header required\"} (2026-09-19)\n- name: X402Payment\n  type: x402\n  version: 2\n  in: header\n  parameter: X-PAYMENT (request) / PAYMENT-REQUIRED (402 challenge response)\n  sources:\n  - https://agenthealthmonitor.xyz/.well-known/x402\n  - live 402 on GET /risk/{address}, GET /ahs/route/policy, POST verify /v1/outputs\n  applies_to: the 15 payable resources in /.well-known/x402 (all 14 documented endpoints plus PUT /ahs/route/policy)\
  \ and AHM\n    Verify POST /v1/outputs\n  network: eip155:8453 (Base mainnet)\n  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (EIP-712 domain name \"USD Coin\" version \"2\")\n  scheme: exact\n  pay_to:\n    main_api: '0xaD64EFCe9CfeE4d1D1701d9a0009CCa72B9ff000'\n    ahm_verify: '0x23A2e9Cd7F0a602A3FcFFaf8074113A9205726E5'\n  facilitator: https://facilitator.payai.network\n  max_timeout_seconds: 300\n  flow: 1) call the endpoint; 2) receive 402 with body {} and PAYMENT-REQUIRED = base64 JSON {x402Version 2, error \"Payment\n    required\", resource{url, description, mimeType}, accepts[{scheme, network, asset, amount, payTo, maxTimeoutSeconds, extra}],\n    extensions.bazaar}; 3) sign an EIP-3009 transferWithAuthorization for accepts[0]; 4) resend with X-PAYMENT; the facilitator\n    verifies and settles.\n  identity: 'The payer wallet address becomes the caller identity for stateful routes (routing policy owner, batch limits)\n    — \"x402 callers: owner_id = lowercased payer\
  \ wallet\" in source.'\n  observed: GET /risk/0x0000000000000000000000000000000000000001 -> 402, accepts[0].amount 1000 (= $0.001); GET /ahs/route/policy\n    -> 402 amount 10000; POST https://verify.agenthealthmonitor.xyz/v1/outputs -> 402 amount 500000 (2026-09-19)\n- name: InternalKey\n  type: apiKey\n  in: header\n  parameter: X-Internal-Key\n  sources:\n  - 'openapi operation descriptions (Admin tag: \"Protected by X-Internal-Key header. Not accessible via x402 payment.\")'\n  applies_to:\n  - security_activity_security_activity_get\n  - trust_registry_trust_registry_get\n  - internal_agent_profile_internal_agent_profile__address__get\n  - trigger_acp_scan_acp_scan_trigger_post\n  - acp_scan_status_acp_scan_status_get\n  - trigger_olas_scan_olas_scan_trigger_post\n  - olas_scan_status_olas_scan_status_get\n  - trigger_arc_scan_arc_scan_trigger_post\n  - arc_scan_status_arc_scan_status_get\n  - trigger_celo_scan_celo_scan_trigger_post\n  - celo_scan_status_celo_scan_status_get\n  -\
  \ trigger_erc8004_scan_erc8004_scan_trigger_post\n  - erc8004_scan_status_erc8004_scan_status_get\n  - erc8183_status_erc8183_status_get\n  note: Operator-only; also bypasses x402 on paid routes (source). Not obtainable by customers.\n  observed: GET /trust-registry -> 401 {\"detail\":\"Unauthorized\"}\n- name: CouponCode\n  type: path-token\n  in: path\n  parameter: '{code} in /coupon/{action}/{code}/{address}'\n  sources:\n  - 'openapi info.description: \"partners can use coupon codes to access any paid endpoint without x402 payment\"'\n  applies_to:\n  - validate_coupon_coupon_validate__code__get\n  - coupon_risk_coupon_risk__code___address__get\n  - coupon_health_coupon_health__code___address__get\n  - coupon_optimize_coupon_optimize__code___address__get\n  - coupon_retry_coupon_retry__code___address__get\n  - coupon_protect_coupon_protect__code___address__get\n  - coupon_alerts_coupon_alerts__code___address__get\n  - coupon_premium_risk_coupon_risk_premium__code___address__get\n \
  \ - coupon_counterparties_coupon_counterparties__code___address__get\n  - coupon_network_map_coupon_network_map__code___address__get\n  - coupon_wash_coupon_wash__code___address__get\n  - coupon_ahs_coupon_ahs__code___address__get\n  - coupon_report_card_coupon_report_card__code___address__get\n  note: Partner-issued codes; rate-limited to 5 attempts per window on validation and access (source). A credential in the\n    URL path, so it appears in logs and caches.\nagent_card_auth:\n  note: The A2A card (a2a/agenthealthmonitor-xyz-agent-card.json) declares bearerAuth (http bearer, JWT) and an apiKey header\n    named X-AHM-API-Key — neither matches the deployed REST API, which uses X-API-Key and no bearer tokens; the A2A endpoint\n    the card protects is not deployed.\nsdk:\n  ahm-shield: AHMShield(api_key=\"ahm_live_...\") sends X-API-Key; no x402 support in the SDK (an agent paying with x402 uses\n    an x402 HTTP client instead).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/authentication/agenthealthmonitor-xyz-authentication.yml
summary_line: apiKey/x402-payment/internal-key/coupon · 4 schemes
tags:
- Agents
- Agent Trust
- Risk Scoring
- Wallet Intelligence
- Blockchain
- Base
- x402
- Agentic Commerce
- Monitoring
- Webhook
- Web3
- Verifiable Credentials
- Developer Tools
- agent-native
---
