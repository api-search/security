---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hergertsynthora-com-mesh-aggregate-openapi.yml
  format: yaml
  label: SYNTHORA Machine-Payable API Mesh
  slug: synthora-machine-payable-api-mesh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hergertsynthora-com/refs/heads/main/openapi/hergertsynthora-com-mesh-aggregate-openapi.yml
- filename: hergertsynthora-com-agent-notary-openapi.yml
  format: yaml
  label: SYNTHORA Agent Notary
  slug: synthora-agent-notary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hergertsynthora-com/refs/heads/main/openapi/hergertsynthora-com-agent-notary-openapi.yml
- filename: hergertsynthora-com-agentcard-openapi.json
  format: json
  label: SYNTHORA x402 Per-Service Contracts
  slug: synthora-x402-per-service-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hergertsynthora-com/refs/heads/main/openapi/services/hergertsynthora-com-agentcard-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Hergertsynthora Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hergert Synthora secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hergert Synthora
provider_slug: hergertsynthora-com
scheme_count: 3
schemes:
- applies_to: every paid operation (global security in the aggregate; implied by x-payment-info in every per-service spec)
  description: 'EIP-3009 transferWithAuthorization payload, USDC on Base (eip155:8453). Obtained by first calling the endpoint and reading the 402 challenge (accepts[] in the body; the same JSON base64url in the payment-required header; on the api gateway also a WWW-Authenticate: x402 network=..., asset=..., pay_to=..., max_amount=..., resource=... challenge).'
  in: header
  name: x402Payment
  parameter: X-PAYMENT
  sources:
  - openapi/hergertsynthora-com-mesh-aggregate-openapi.yml
  - live 402 on https://api.hergertsynthora.com/v1/wallet-enrich and https://notary.hergertsynthora.com/service
  type: apiKey
- description: 'How the agent cards declare the same requirement: "Pago por llamada x402: USDC en Base (eip155:8453). La primera llamada devuelve HTTP 402 con los terminos de pago; el pago se verifica on-chain y la respuesta incluye recibo firmado." Not an IANA-registered HTTP auth scheme; recorded because the live gateway does emit a WWW-Authenticate challenge with that token.'
  name: x402
  scheme: x402
  sources:
  - a2a/hergertsynthora-com-agent-card.json (securitySchemes.x402)
  - a2a/hergertsynthora-com-notary-agent-card.json (securitySchemes.x402)
  type: http
- description: 'The caller''s Base address (0x...). Two uses the provider documents: (1) free trial - send it instead of a payment and the product answers up to x-free-tier calls (1 or 3, per product) without charge; (2) the "nucleo" state and meshgraph endpoints treat it as an API key and answer 403 without it (docs section 02; the docs elide the host for those endpoints).'
  in: header
  name: wallet
  parameter: X-WALLET
  sources:
  - a2a/hergertsynthora-com-agent-card.json (securitySchemes.wallet)
  - https://hergertsynthora.com/api/
  - https://api.hergertsynthora.com/llms.txt
  - 402 body freeTier {callsPerWallet, header X-WALLET}; response header x-free-tier
  type: apiKey
slug: hergertsynthora-com-authentication
source_filename: hergertsynthora-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  Derived baseline from openapi/hergertsynthora-com-mesh-aggregate-openapi.yml (securitySchemes.x402Payment) by\n  0-working/derive-authentication.py, then upgraded from the provider's own auth statements: the agent card\n  securitySchemes (x402 http scheme + X-WALLET apiKey), https://hergertsynthora.com/api/ (X-WALLET on core\n  endpoints, 403 without it), https://api.hergertsynthora.com/llms.txt (free tier), the notary card and the live\n  402 responses observed 2026-09-19 (WWW-Authenticate x402 challenge, payment-required header, x-free-tier).\ndocs: https://hergertsynthora.com/api/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Wallet-native, accountless. There is no sign-up, no API key issuance and no OAuth. A paid call authenticates\n    itself by carrying a payment (X-PAYMENT); an unpaid trial call identifies itself by its wallet address\n    (X-WALLET). The 59 per-service\
  \ OpenAPIs and the notary spec declare NO securitySchemes at all - the\n    requirement lives in info.x-payment / x-payment-info and the 402 response.\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: >-\n    EIP-3009 transferWithAuthorization payload, USDC on Base (eip155:8453). Obtained by first calling the\n    endpoint and reading the 402 challenge (accepts[] in the body; the same JSON base64url in the\n    payment-required header; on the api gateway also a WWW-Authenticate: x402 network=..., asset=..., pay_to=...,\n    max_amount=..., resource=... challenge).\n  applies_to: every paid operation (global security in the aggregate; implied by x-payment-info in every per-service spec)\n  sources:\n  - openapi/hergertsynthora-com-mesh-aggregate-openapi.yml\n  - live 402 on https://api.hergertsynthora.com/v1/wallet-enrich and https://notary.hergertsynthora.com/service\n- name: x402\n  type: http\n  scheme: x402\n  description: >-\n    How\
  \ the agent cards declare the same requirement: \"Pago por llamada x402: USDC en Base (eip155:8453). La\n    primera llamada devuelve HTTP 402 con los terminos de pago; el pago se verifica on-chain y la respuesta\n    incluye recibo firmado.\" Not an IANA-registered HTTP auth scheme; recorded because the live gateway does\n    emit a WWW-Authenticate challenge with that token.\n  sources:\n  - a2a/hergertsynthora-com-agent-card.json (securitySchemes.x402)\n  - a2a/hergertsynthora-com-notary-agent-card.json (securitySchemes.x402)\n- name: wallet\n  type: apiKey\n  in: header\n  parameter: X-WALLET\n  description: >-\n    The caller's Base address (0x...). Two uses the provider documents: (1) free trial - send it instead of a\n    payment and the product answers up to x-free-tier calls (1 or 3, per product) without charge; (2) the\n    \"nucleo\" state and meshgraph endpoints treat it as an API key and answer 403 without it (docs section 02;\n    the docs elide the host for those endpoints).\n\
  \  sources:\n  - a2a/hergertsynthora-com-agent-card.json (securitySchemes.wallet)\n  - https://hergertsynthora.com/api/\n  - https://api.hergertsynthora.com/llms.txt\n  - 402 body freeTier {callsPerWallet, header X-WALLET}; response header x-free-tier\ncredentials:\n  sign_up: none - no accounts; the wallet is the identity\n  key_prefixes: none\n  rotation: n/a\n  sandbox_keys: none (see sandbox/hergertsynthora-com-sandbox.yml)\ntransport:\n  https_only: true\n  tls: TLSv1.3 on apex, api and notary hosts (security/hergertsynthora-com-domain-security.yml)\n  mcp: https://mcp.hergertsynthora.com/mcp - initialize and tools/list are anonymous; tools/call is x402-paid; no OAuth metadata served\n  a2a: https://api.hergertsynthora.com/a2a - JSON-RPC, same x402 / X-WALLET model per the card's security[]\ngaps:\n- The per-service and notary OpenAPIs declare no securitySchemes, so a generic OpenAPI client sees them as unauthenticated.\n- The X-WALLET \"nucleo\" endpoints are documented without a\
  \ host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hergertsynthora-com/refs/heads/main/authentication/hergertsynthora-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Agents
- A2A
- MCP
- x402
- Web3
- Intelligence
- Sanctions Screening
- Prediction Markets
- OSINT
- Blockchain
- Spain
---
