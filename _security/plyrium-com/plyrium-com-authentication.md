---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plyrium-com-vouchspec-openapi.yml
  format: yaml
  label: VouchSpec Agent Skill Evidence API
  slug: vouchspec-agent-skill-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/openapi/plyrium-com-vouchspec-openapi.yml
auth_types: []
description: 'VouchSpec has no login, API-key signup or OAuth. The read surface is anonymous. The single write operation is gated by PAYMENT, not identity: an x402 v2 challenge-and-retry on POST /api/vouchspec/v1/validate. Credentials exist only AFTER settlement - the 200 response hands back a one-time tenant API key and a one-time delivery token, which together unlock that order''s result. The OpenAPI declares no securitySchemes because none of its eight operations takes a credential up front; derive-authentication.py therefore produced no profile and this file is authored from the provider''s discovery contract instead.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Plyrium Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plyrium declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Plyrium
provider_slug: plyrium-com
scheme_count: 3
schemes:
- amount: '0.25'
  applies_to:
  - purchaseExactCommitValidation
  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)
  atomic_amount: '250000'
  authentication_before_payment: false
  challenge:
    body: JSON with error.code payment_required, accepts[], and an extensions.bazaar block carrying a full example request body
    header: PAYMENT-REQUIRED (base64 x402 v2 payment requirements)
    observed: 2026-09-19 - an empty unpaid POST returned exactly this (documented as the sanctioned challenge-discovery probe)
    status: 402
  facilitator: https://api.cdp.coinbase.com/platform/v2/x402
  human_checkout: false
  max_timeout_seconds: 300
  name: x402-payment
  network: eip155:8453 (Base mainnet)
  note: Exact payment retries return the same credentials (discovery acquisition.exact_payment_retries_return_same_credentials true)
  pay_to: '0x5AbA743d6e6Dc22584D9e175D0b39E972AB9918d'
  protocol: x402
  registration_required: false
  retry:
    header: PAYMENT-SIGNATURE (base64 x402 v2 authorization, maxLength 16384, supplied only on the paid retry)
    response_header: PAYMENT-RESPONSE (base64 settlement response on 200)
  scheme: exact
  type: payment-gated
  version: 2
- applies_to: order and result endpoints returned in PaidValidationAccess.endpoints (order_template, result_template, rotate/revoke delivery-token templates - not in the public OpenAPI)
  header: 'Authorization: Bearer {tenant_api_key}'
  issued_by: purchaseExactCommitValidation 200 response (PaidValidationAccess.credentials.tenant_api_key)
  name: tenant-bearer
  scheme: bearer
  shown_once: true
  stored_as: keyed digest (never plaintext) - policies page "Credential handling"
  type: http
- applies_to: the same order/result endpoints, REQUIRED TOGETHER with the tenant bearer ("A result requires both credentials")
  expires: yes - delivery_token_expires_at in the response; payment-flow.md states delivery capabilities expire after 30 days and may be rotated or revoked
  header: X-VouchSpec-Delivery-Token
  in: header
  issued_by: purchaseExactCommitValidation 200 response (PaidValidationAccess.credentials.delivery_token + delivery_token_expires_at)
  name: delivery-token
  shown_once: true
  type: apiKey
slug: plyrium-com-authentication
source_filename: plyrium-com-authentication.yml
source_heading: Authentication Profile
source_url: https://vouchspec.plyrium.com/api/vouchspec/v1/discovery (authentication + acquisition + payment blocks)
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://vouchspec.plyrium.com/api/vouchspec/v1/discovery\ndocs: https://vouchspec.plyrium.com/api/vouchspec/v1/discovery\nsources:\n- https://vouchspec.plyrium.com/api/vouchspec/v1/discovery (authentication + acquisition + payment blocks)\n- https://vouchspec.plyrium.com/openapi.json (no securitySchemes declared; PAYMENT-SIGNATURE header parameter; PaidValidationAccess.credentials schema)\n- https://vouchspec.plyrium.com/.well-known/x402 (payTo, facilitator, network)\n- https://www.plyrium.com/vouchspec/policies (\"Credential handling\")\n- https://raw.githubusercontent.com/mordiaky/vouchspec/main/docs/payment-flow.md (order/result credential pairing, 30-day delivery capability expiry)\ndescription: >-\n  VouchSpec has no login, API-key signup or OAuth. The read surface is anonymous. The single write operation is\n  gated by PAYMENT, not identity: an x402 v2 challenge-and-retry on POST /api/vouchspec/v1/validate. Credentials\n\
  \  exist only AFTER settlement - the 200 response hands back a one-time tenant API key and a one-time delivery\n  token, which together unlock that order's result. The OpenAPI declares no securitySchemes because none of its\n  eight operations takes a credential up front; derive-authentication.py therefore produced no profile and this\n  file is authored from the provider's discovery contract instead.\nanonymous_surface:\n  operations: [getVouchSpecHealth, getVouchSpecDiscovery, getVouchSpecX402Manifest, getVouchSpecValidationService, getVouchSpecIssuerKey, getVouchSpecReceipt, getVouchSpecReceiptStatus]\n  observed: every one answered 200 with no credential on 2026-09-19; response header x-plyrium-auth-bypass anonymous-public\n  mcp: https://vouchspec.plyrium.com/api/vouchspec/v1/mcp - tools/list and tools/call anonymous\n  a2a: https://vouchspec.plyrium.com/api/vouchspec/v1/a2a - message/send anonymous\nschemes:\n- name: x402-payment\n  type: payment-gated\n  applies_to: [purchaseExactCommitValidation]\n\
  \  protocol: x402\n  version: 2\n  scheme: exact\n  network: eip155:8453 (Base mainnet)\n  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)\n  amount: '0.25'\n  atomic_amount: '250000'\n  pay_to: '0x5AbA743d6e6Dc22584D9e175D0b39E972AB9918d'\n  facilitator: https://api.cdp.coinbase.com/platform/v2/x402\n  max_timeout_seconds: 300\n  challenge:\n    status: 402\n    header: PAYMENT-REQUIRED (base64 x402 v2 payment requirements)\n    body: JSON with error.code payment_required, accepts[], and an extensions.bazaar block carrying a full example request body\n    observed: 2026-09-19 - an empty unpaid POST returned exactly this (documented as the sanctioned challenge-discovery probe)\n  retry:\n    header: PAYMENT-SIGNATURE (base64 x402 v2 authorization, maxLength 16384, supplied only on the paid retry)\n    response_header: PAYMENT-RESPONSE (base64 settlement response on 200)\n  registration_required: false\n  authentication_before_payment: false\n  human_checkout: false\n  note: Exact\
  \ payment retries return the same credentials (discovery acquisition.exact_payment_retries_return_same_credentials true)\n- name: tenant-bearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer {tenant_api_key}'\n  issued_by: purchaseExactCommitValidation 200 response (PaidValidationAccess.credentials.tenant_api_key)\n  shown_once: true\n  stored_as: keyed digest (never plaintext) - policies page \"Credential handling\"\n  applies_to: order and result endpoints returned in PaidValidationAccess.endpoints (order_template, result_template, rotate/revoke delivery-token templates - not in the public OpenAPI)\n- name: delivery-token\n  type: apiKey\n  in: header\n  header: X-VouchSpec-Delivery-Token\n  issued_by: purchaseExactCommitValidation 200 response (PaidValidationAccess.credentials.delivery_token + delivery_token_expires_at)\n  shown_once: true\n  expires: yes - delivery_token_expires_at in the response; payment-flow.md states delivery capabilities expire after 30 days\
  \ and may be rotated or revoked\n  applies_to: the same order/result endpoints, REQUIRED TOGETHER with the tenant bearer (\"A result requires both credentials\")\nidempotency_header: 'Idempotency-Key: {unique_8_to_128_character_value}' # documented for authenticated tenant operations; see conventions/\nresult_authentication:\n  media_type: application/vnd.dsse.envelope.v1+json\n  signature: Ed25519 over exact DSSE payload bytes\n  issuer_key: https://vouchspec.plyrium.com/api/vouchspec/v1/keys/issuer (key_id m3Vz2bX1-lZ-osJb91mHCNE_-Lehx2fFc2TvExDbbn0, RFC 8037 OKP JWK)\n  note: The receipt itself is the authenticated object; public receipt bytes need no credential, and the no-store /status endpoint carries live invalidation.\ngaps:\n- The OpenAPI declares no securitySchemes at all, so a generic client cannot learn from the spec alone that POST /validate is x402-gated; the x-x402 and x-vouchspec extensions and the 402 response carry that information instead.\n- The credentialed order/result/rotate/revoke\
  \ endpoints are named in discovery (route templates) but are absent from the OpenAPI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/authentication/plyrium-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Agent Skills
- Supply Chain Security
- Software Provenance
- x402
- Agentic Commerce
- A2A
- MCP
- Field Service
- Home Services
---
