---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getaiscan-app-openapi.json
  format: json
  label: AIScan Agent API
  slug: aiscan-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaiscan-app/refs/heads/main/openapi/getaiscan-app-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Getaiscan App Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIScan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIScan
provider_slug: getaiscan-app
scheme_count: 1
schemes:
- applied_to: every POST /api/agent/{capability} operation (19 of 20 operations); the operations declare no per-operation security[] and the document declares no top-level security, so the requirement is expressed by the 402 response each operation declares rather than by a security requirement object
  challenge_observed:
    body_fields:
    - x402Version
    - error
    - resource
    - accepts
    - extensions
    - price
    - currency
    - recipient
    - instructions
    - capability
    - index
    headers:
      payment-required: base64 JSON — {x402Version 2, error "PAYMENT-SIGNATURE header is required", resource {url, description, mimeType}, accepts [{scheme exact, network eip155:8453, amount 60000, asset, payTo, maxTimeoutSeconds 300, extra {name USD Coin, version 2}}], extensions {}}
      x-payment-amount: '0.06'
      x-payment-asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
      x-payment-currency: USDC
      x-payment-network: eip155:8453
      x-payment-recipient: '0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7'
      x-payment-required: 'true'
      x-payment-version: '2'
    instructions_verbatim: 'Pay 0.06 USDC: x402 V2 ''exact'' scheme (PAYMENT-SIGNATURE header, settled via Coinbase CDP facilitator), or direct-transfer: send 0.06 USDC on Base (eip155:8453) to 0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7 and retry with PAYMENT-SIGNATURE: <tx_hash>'
    note: The body's accepts[0].network says "base" while the header and the PAYMENT-REQUIRED payload say "eip155:8453"; the amount is in USDC base units (60000 = 0.06 USDC, 6 decimals).
    request: POST https://api.getaiscan.app/api/agent/check_health {"url":"https://example.com"} with no payment header, 2026-09-19
    status: 402
  description: 'x402 V2 payment: signed payload or Base USDC tx hash'
  exempt:
  - index
  header_aliases:
    accepted_by_cors:
    - PAYMENT-SIGNATURE
    - Payment-Signature
    - X-Payment
    - X-PAYMENT
    note: The legacy agent.json descriptor and the mcp.json descriptor name X-Payment; the OpenAPI, the agent card and the live challenge name PAYMENT-SIGNATURE. Use PAYMENT-SIGNATURE.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  protocol:
    asset: USDC — 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
    flows:
    - description: EIP-3009 transferWithAuthorization signed by the payer, settled via the Coinbase CDP facilitator; the signed payload goes in PAYMENT-SIGNATURE.
      id: exact
    - description: Send the exact USDC amount on Base to pay_to, then retry the same request with PAYMENT-SIGNATURE set to the transaction hash.
      id: direct-transfer
    max_timeout_seconds: 300
    name: x402
    network: eip155:8453 (Base mainnet)
    pay_to: '0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7'
    version: 2
  semantics: payment credential, not an identity credential — the paying wallet is the only identity the API sees
  sources:
  - openapi/getaiscan-app-openapi.json
  type: apiKey
slug: getaiscan-app-authentication
source_filename: getaiscan-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/getaiscan-app-openapi.json\ndocs:\n- https://getaiscan.app/llms.txt\n- https://api.getaiscan.app/api/agent/index\n- https://getaiscan.app/.well-known/agent-card.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 1\n  headline: >-\n    No API key, no account, no signup, no OAuth. The single securityScheme in the contract is named \"x402\" and\n    typed apiKey-in-header only because OpenAPI has no vocabulary for a payment credential: the header\n    PAYMENT-SIGNATURE carries an x402 V2 payment — either a signed EIP-3009 \"exact\" authorization for USDC on\n    Base settled through the Coinbase CDP facilitator, or the transaction hash of a direct USDC transfer to the\n    provider's wallet. An unpaid call to any paid route returns HTTP 402 with a base64 PAYMENT-REQUIRED header\n    and a JSON body naming the price, asset, network, recipient and both\
  \ flows. GET /api/agent/index is the only\n    unauthenticated route (security: []).\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: 'x402 V2 payment: signed payload or Base USDC tx hash'\n  semantics: payment credential, not an identity credential — the paying wallet is the only identity the API sees\n  protocol:\n    name: x402\n    version: 2\n    network: eip155:8453 (Base mainnet)\n    asset: USDC — 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n    pay_to: '0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7'\n    flows:\n    - id: exact\n      description: EIP-3009 transferWithAuthorization signed by the payer, settled via the Coinbase CDP facilitator; the signed payload goes in PAYMENT-SIGNATURE.\n    - id: direct-transfer\n      description: Send the exact USDC amount on Base to pay_to, then retry the same request with PAYMENT-SIGNATURE set to the transaction hash.\n    max_timeout_seconds: 300\n  challenge_observed:\n    request: 'POST\
  \ https://api.getaiscan.app/api/agent/check_health {\"url\":\"https://example.com\"} with no payment header, 2026-09-19'\n    status: 402\n    headers:\n      payment-required: base64 JSON — {x402Version 2, error \"PAYMENT-SIGNATURE header is required\", resource {url, description, mimeType}, accepts [{scheme exact, network eip155:8453, amount 60000, asset, payTo, maxTimeoutSeconds 300, extra {name USD Coin, version 2}}], extensions {}}\n      x-payment-required: 'true'\n      x-payment-version: '2'\n      x-payment-amount: '0.06'\n      x-payment-currency: USDC\n      x-payment-network: eip155:8453\n      x-payment-recipient: '0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7'\n      x-payment-asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n    body_fields: [x402Version, error, resource, accepts, extensions, price, currency, recipient, instructions, capability, index]\n    instructions_verbatim: >-\n      Pay 0.06 USDC: x402 V2 'exact' scheme (PAYMENT-SIGNATURE header, settled via Coinbase\
  \ CDP facilitator),\n      or direct-transfer: send 0.06 USDC on Base (eip155:8453) to 0x0a28ace35b9687a9334cd503b3c7d4b23734a1c7\n      and retry with PAYMENT-SIGNATURE: <tx_hash>\n    note: The body's accepts[0].network says \"base\" while the header and the PAYMENT-REQUIRED payload say \"eip155:8453\"; the amount is in USDC base units (60000 = 0.06 USDC, 6 decimals).\n  header_aliases:\n    accepted_by_cors: [PAYMENT-SIGNATURE, Payment-Signature, X-Payment, X-PAYMENT]\n    note: The legacy agent.json descriptor and the mcp.json descriptor name X-Payment; the OpenAPI, the agent card and the live challenge name PAYMENT-SIGNATURE. Use PAYMENT-SIGNATURE.\n  applied_to: every POST /api/agent/{capability} operation (19 of 20 operations); the operations declare no per-operation security[] and the document declares no top-level security, so the requirement is expressed by the 402 response each operation declares rather than by a security requirement object\n  exempt: [index]\n  sources:\n \
  \ - openapi/getaiscan-app-openapi.json\ngaps:\n- The OpenAPI declares the x402 scheme in components.securitySchemes but applies it nowhere (no top-level or per-operation security[] except index's empty list); a client generator will treat every operation as anonymous.\n- No OAuth/OIDC, no RFC 9728 protected-resource metadata, no RFC 8414 metadata on either host; there is nothing to discover beyond the 402 itself.\n- No testnet or sandbox payment path is documented; every call is a real mainnet USDC payment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaiscan-app/refs/heads/main/authentication/getaiscan-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Visibility
- Website Auditing
- SEO
- Answer Engine Optimization
- Generative Engine Optimization
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Agent-Native
---
