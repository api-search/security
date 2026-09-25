---
anonymous_access: true
api_key_in: []
api_specs:
- filename: 558686-xyz-gpt55-model-gateway-openapi.json
  format: json
  label: GPT55 Model Gateway API
  slug: gpt55-model-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-gpt55-model-gateway-openapi.json
- filename: 558686-xyz-api-market-utility-tools-openapi.json
  format: json
  label: GPT-5.5 Utility Tools for API.market
  slug: gpt55-utility-tools-api-market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-api-market-utility-tools-openapi.json
- filename: 558686-xyz-sub2api-openapi.json
  format: json
  label: Sub2API OpenAI-compatible API
  slug: sub2api-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-sub2api-openapi.json
auth_types:
- x402-payment
- http-bearer
- api-key-header
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: 558686 Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: gpt55-token-gateway secures its APIs with x402-payment, http-bearer, and api-key-header across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: gpt55-token-gateway
provider_slug: 558686-xyz
scheme_count: 4
schemes:
- account_required: false
  api: GPT55 Model Gateway API (gpt55.558686.xyz)
  api_key_required: false
  applies_to: all 36 paid operations; GET /v1/models is anonymous
  client_libraries_named:
  - '@x402/fetch + @x402/evm + viem (buyer guide quickstart)'
  - first-payment-client.mjs (provider script, quote-only by default; PAY_REAL_X402=1 + EVM_PRIVATE_KEY in the buyer process to pay)
  declared_in_spec: false
  declared_in_spec_note: The GPT55 OpenAPI declares no securitySchemes; the 402 response on 36 of 37 operations and x-x402-price are the only in-contract signals. overlays/558686-xyz-gpt55-model-gateway-overlay.yaml adds an apiKey-in-header scheme named x402Payment as the closest OpenAPI expression.
  flow_verbatim:
  - Send the intended HTTP request without a payment header.
  - Read the HTTP 402 response and its accepts array.
  - Select the exact accept requirement and generate the x402 payment header with your Base USDC wallet.
  - Retry the same request with the payment header.
  - Read the payment response header and JSON body. Successful paid model calls return OpenAI-compatible JSON.
  header: X-PAYMENT
  in: header
  kyc_required: false
  name: x402Payment
  private_key_sent_to_service: false
  requirement_observed:
    asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC)
    facilitator: provider-pool (xpay active)
    maxTimeoutSeconds: 300
    network: eip155:8453
    payTo: '0x1f0130669ca6fd02e025a984cc038f139df19a2f'
    scheme: exact
  response_headers:
  - PAYMENT-REQUIRED
  - X-PAYMENT-REQUIRED
  - PAYMENT-RESPONSE
  - X-PAYMENT-RESPONSE
  - x-x402-receipt-id
  - x-x402-receipt-url
  type: x402
  version: '2'
- api: GPT55 Model Gateway API (gpt55.558686.xyz)
  declared_in_spec: false
  name: operatorBearer
  note: Recorded because the provider documents it; there is no way for a member of the public to obtain one. An unpaid request with an invalid X-PAYMENT header returned the ordinary 402 quote, not a 401.
  public: false
  scheme: bearer
  type: http
  verbatim: A private Bearer token is also accepted for owner/admin testing.
  verbatim_2: Private Bearer keys are only an operator bypass; public buyers should use the x402 quote and payment flow.
- api: GPT55 discovery surface + GPT-5.5 Utility Tools for API.market (gpt55.558686.xyz/api-market)
  declared_in_spec: api-market OpenAPI declares no securitySchemes; its description says commercial access is configured in API.market
  name: none
  observed: GET /api-market/v1/tools/timestamp and /text-stats answered 200 with no credential and no payment (2026-09-20); GET /v1/models, MCP initialize/tools/list/resources/list and every manifest likewise anonymous.
  type: none
- alternate_carriers:
  - x-api-key header
  - query key (named in the 401 message, truncated in the observed body)
  api: Sub2API OpenAI-compatible API (sub2api.558686.xyz, api.558686.xyz)
  applies_to: all three operations (GET /v1/models, POST /v1/chat/completions, POST /v1/responses)
  base_url_for_clients: https://sub2api.558686.xyz/v1
  bearerFormat: API key
  declared_in_spec: true
  errors:
    invalid: 401 {"code":"INVALID_API_KEY","message":"Invalid API key"}
    missing: 401 {"code":"API_KEY_REQUIRED","message":"API key is required in Authorization header (Bearer scheme), x-api-key header, or ..."}
  key_issuance: 'Console https://sub2api.558686.xyz/keys after email registration + verification; docs: "创建成功后立即保存完整 Key，它通常只会完整显示一次" (the full key is normally shown only once). Registration is CLOSED per /verify-models (registration_enabled=false, google_oauth_enabled=false); "contact the administrator for a test key".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/558686-xyz-sub2api-openapi.json
  type: http
slug: 558686-xyz-authentication
source_filename: 558686-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  Derived baseline from openapi/558686-xyz-sub2api-openapi.json (the only spec with a\n  securityScheme) by derive-authentication.py, then upgraded from the provider docs:\n  https://gpt55.558686.xyz/buyer-guide (\"No account, subscription, or public API key is required\n  for public paid calls\"; \"Integration flow\"), /llms-full.txt (\"A private Bearer token is also\n  accepted for owner/admin testing\"), /mcp/config (authentication block), /.well-known/x402\n  (payment, settlement, privateKeySentToService), SECURITY.md (\"The service never needs a buyer's\n  private key\"), the live 402 and 401 responses observed 2026-09-20, and the Sub2API docs\n  https://sub2api.558686.xyz/docs/getting-started.html and /docs/register-guide.html.\ndocs:\n  - https://gpt55.558686.xyz/buyer-guide\n  - https://gpt55.558686.xyz/x402/guides/ai-agent-x402-api\n  - https://sub2api.558686.xyz/docs/getting-started.html\nchecked: '2026-09-19'\n\
  summary:\n  types: [x402-payment, http-bearer, api-key-header]\n  note: >-\n    Two different models on two hosts. GPT55 has NO identity credential for the public: every\n    paid route is gated by an x402 payment presented in the X-PAYMENT header after a 402 quote,\n    and the discovery/metadata surface (GET /v1/models, MCP initialize/tools/list/resources/list,\n    every JSON manifest, the /api-market utilities) is fully anonymous. A private Bearer token\n    exists but is documented as an operator-only bypass, not a public option. Sub2API is a\n    conventional API-key relay: Authorization: Bearer <key> (also x-api-key or a query key),\n    with keys created in a console whose self-service registration is currently closed.\n  no_oauth: 'No OAuth 2.0, OIDC, scopes, RFC 8414 or RFC 9728 metadata anywhere; scopes/ is therefore not emitted.'\nschemes:\n- name: x402Payment\n  api: GPT55 Model Gateway API (gpt55.558686.xyz)\n  type: x402\n  version: '2'\n  in: header\n  header: X-PAYMENT\n\
  \  declared_in_spec: false\n  declared_in_spec_note: 'The GPT55 OpenAPI declares no securitySchemes; the 402 response on 36 of 37 operations and x-x402-price are the only in-contract signals. overlays/558686-xyz-gpt55-model-gateway-overlay.yaml adds an apiKey-in-header scheme named x402Payment as the closest OpenAPI expression.'\n  flow_verbatim:\n    - 'Send the intended HTTP request without a payment header.'\n    - 'Read the HTTP 402 response and its accepts array.'\n    - 'Select the exact accept requirement and generate the x402 payment header with your Base USDC wallet.'\n    - 'Retry the same request with the payment header.'\n    - 'Read the payment response header and JSON body. Successful paid model calls return OpenAI-compatible JSON.'\n  requirement_observed: {scheme: exact, network: 'eip155:8453', asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC)', payTo: '0x1f0130669ca6fd02e025a984cc038f139df19a2f', maxTimeoutSeconds: 300, facilitator: 'provider-pool (xpay active)'}\n\
  \  response_headers: [PAYMENT-REQUIRED, X-PAYMENT-REQUIRED, PAYMENT-RESPONSE, X-PAYMENT-RESPONSE, x-x402-receipt-id, x-x402-receipt-url]\n  account_required: false\n  api_key_required: false\n  kyc_required: false\n  private_key_sent_to_service: false\n  client_libraries_named: ['@x402/fetch + @x402/evm + viem (buyer guide quickstart)', 'first-payment-client.mjs (provider script, quote-only by default; PAY_REAL_X402=1 + EVM_PRIVATE_KEY in the buyer process to pay)']\n  applies_to: all 36 paid operations; GET /v1/models is anonymous\n- name: operatorBearer\n  api: GPT55 Model Gateway API (gpt55.558686.xyz)\n  type: http\n  scheme: bearer\n  declared_in_spec: false\n  public: false\n  verbatim: 'A private Bearer token is also accepted for owner/admin testing.'\n  verbatim_2: 'Private Bearer keys are only an operator bypass; public buyers should use the x402 quote and payment flow.'\n  note: 'Recorded because the provider documents it; there is no way for a member of the public to obtain\
  \ one. An unpaid request with an invalid X-PAYMENT header returned the ordinary 402 quote, not a 401.'\n- name: none\n  api: 'GPT55 discovery surface + GPT-5.5 Utility Tools for API.market (gpt55.558686.xyz/api-market)'\n  type: none\n  declared_in_spec: 'api-market OpenAPI declares no securitySchemes; its description says commercial access is configured in API.market'\n  observed: 'GET /api-market/v1/tools/timestamp and /text-stats answered 200 with no credential and no payment (2026-09-20); GET /v1/models, MCP initialize/tools/list/resources/list and every manifest likewise anonymous.'\n- name: bearerAuth\n  api: Sub2API OpenAI-compatible API (sub2api.558686.xyz, api.558686.xyz)\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  declared_in_spec: true\n  sources: [openapi/558686-xyz-sub2api-openapi.json]\n  alternate_carriers: ['x-api-key header', 'query key (named in the 401 message, truncated in the observed body)']\n  errors: {missing: '401 {\"code\":\"API_KEY_REQUIRED\"\
  ,\"message\":\"API key is required in Authorization header (Bearer scheme), x-api-key header, or ...\"}', invalid: '401 {\"code\":\"INVALID_API_KEY\",\"message\":\"Invalid API key\"}'}\n  key_issuance: 'Console https://sub2api.558686.xyz/keys after email registration + verification; docs: \"创建成功后立即保存完整 Key，它通常只会完整显示一次\" (the full key is normally shown only once). Registration is CLOSED per /verify-models (registration_enabled=false, google_oauth_enabled=false); \"contact the administrator for a test key\".'\n  base_url_for_clients: https://sub2api.558686.xyz/v1\n  applies_to: all three operations (GET /v1/models, POST /v1/chat/completions, POST /v1/responses)\nmcp:\n  endpoint: https://gpt55.558686.xyz/mcp\n  auth: none for initialize / tools/list / resources/list; tool results are HTTP routes that require the x402 payment above\n  declared: '/mcp/config authentication {type: x402-payment-header, apiKeyRequired: false, accountRequired: false, kycRequired: false, quoteFirst: true}'\na2a:\n\
  \  endpoint: https://gpt55.558686.xyz/a2a\n  auth: 'agent card authentication: [{schemes: [x402]}]; payment.accepts[] carries the requirement'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/authentication/558686-xyz-authentication.yml
summary_line: x402-payment/http-bearer/api-key-header · 4 schemes
tags:
- x402
- Agentic Payments
- MCP
- A2A
- AI Gateway
- OpenAI-Compatible
- LLM
- AI Agents
- USDC
- Base
- API Relay
- Developer Tools
---
