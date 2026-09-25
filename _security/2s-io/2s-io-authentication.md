---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: 2s-io-openapi.json
  format: json
  label: 2s API
  slug: 2s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2s-io/refs/heads/main/openapi/2s-io-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 2S Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: 2s secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 2s
provider_slug: 2s-io
scheme_count: 3
schemes:
- alternate_scheme: upto — on AI endpoints, a Permit2 authorization for the quoted maximum, settled at actual usage; appears as an extra accepts[] entry after exact.
  applied_to: 'all 575 operations (security [{x402Payment: []}] on each; no global security block)'
  description: 'x402 protocol v2: base64-encoded PaymentPayload. Call any paid endpoint without auth to receive a 402 with a multi-network PaymentRequirements envelope. Sign for either rail: EIP-3009 transferWithAuthorization (Base USDC) OR a partial SPL token transfer (Solana USDC). Retry with PAYMENT-SIGNATURE header. X-PAYMENT is also accepted for v1 buyer clients. See https://x402.org.'
  flow:
  - 'Request with no credential → HTTP 402, body = X402PaymentRequiredV2 {x402Version 2, accepts[], resource, error, extensions.bazaar}, header PAYMENT-REQUIRED (same envelope, base64), x-payment-requirements: x402 (observed live 2026-09-19).'
  - 'Sign a USDC authorization for accepts[].amount (atomic units, 6 decimals) on the chosen rail: Base (eip155:8453) EIP-3009 transferWithAuthorization with the EIP-712 domain in accepts[].extra; or Solana (solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp) partial SPL transfer with the feePayer in accepts[].extra.'
  - 'Retry the identical request with PAYMENT-SIGNATURE: <base64 payload> (X-PAYMENT for v1 clients) → 200 + X-PAYMENT-TX. The facilitator (https://api.cdp.coinbase.com/platform/v2/x402) verifies off-chain, the handler runs, settlement follows on-chain and the facilitator pays gas.'
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/2s-io-openapi.json
  - https://2s.io/learn/x402
  type: apiKey
- applied_to: all operations except feedback_send
  description: Bypasses payment for one free real call per endpoint per hour (response marked meta.trial). Not an authentication scheme — an allowance; recorded so an agent knows the anonymous path exists. Declared as components.parameters.TrialMode.
  in: query or header
  name: trial-mode
  parameter: 'trial=1 | X-2s-Trial: 1'
  sources:
  - openapi/2s-io-openapi.json
  - https://2s.io/llms.txt
  type: none
- applied_to: https://2s.io/mcp (hosted MCP server) only
  description: 'The hosted MCP server signs x402 payments on the caller''s behalf, so it takes the caller''s EVM private key (funded with USDC on Base) as a request header. The provider''s own docs warn: "a hosted signer means your key transits 2s infrastructure — for keys that never leave your machine, prefer the local SDK / npx". Not used by the REST API. initialize and tools/list need no header at all.'
  in: header
  name: hosted-mcp-signer
  parameter: X-EVM-Private-Key
  sources:
  - https://2s.io/learn/x402/mcp
  - mcp/2s-io-mcp.yml
  type: apiKey
slug: 2s-io-authentication
source_filename: 2s-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/2s-io-openapi.json\ndocs:\n- https://2s.io/learn/x402\n- https://2s.io/llms.txt\n- https://2s.io/learn/x402/mcp\n- https://2s.io/.well-known/2s-attestation.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Payment in place of authentication. There are no accounts, no API keys to issue, no OAuth and no OIDC —\n    the single securityScheme is an apiKey-typed header that carries a signed x402 payment, applied to all\n    575 operations. Identity, where it matters (wallet-scoped store/lock/queue/watchers), is the address that\n    paid. Anonymous access exists only through trial mode (one free real call per endpoint per hour) and\n    through the free discovery documents.\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  applied_to: 'all 575 operations (security [{x402Payment: []}] on each; no global security block)'\n  description: 'x402 protocol\
  \ v2: base64-encoded PaymentPayload. Call any paid endpoint without auth to receive a 402 with a multi-network PaymentRequirements envelope. Sign for either rail: EIP-3009 transferWithAuthorization (Base USDC) OR a partial SPL token transfer (Solana USDC). Retry with PAYMENT-SIGNATURE header. X-PAYMENT is also accepted for v1 buyer clients. See https://x402.org.'\n  flow:\n  - 'Request with no credential → HTTP 402, body = X402PaymentRequiredV2 {x402Version 2, accepts[], resource, error, extensions.bazaar}, header PAYMENT-REQUIRED (same envelope, base64), x-payment-requirements: x402 (observed live 2026-09-19).'\n  - 'Sign a USDC authorization for accepts[].amount (atomic units, 6 decimals) on the chosen rail: Base (eip155:8453) EIP-3009 transferWithAuthorization with the EIP-712 domain in accepts[].extra; or Solana (solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp) partial SPL transfer with the feePayer in accepts[].extra.'\n  - 'Retry the identical request with PAYMENT-SIGNATURE: <base64 payload>\
  \ (X-PAYMENT for v1 clients) → 200 + X-PAYMENT-TX. The facilitator (https://api.cdp.coinbase.com/platform/v2/x402) verifies off-chain, the handler runs, settlement follows on-chain and the facilitator pays gas.'\n  alternate_scheme: 'upto — on AI endpoints, a Permit2 authorization for the quoted maximum, settled at actual usage; appears as an extra accepts[] entry after exact.'\n  sources:\n  - openapi/2s-io-openapi.json\n  - https://2s.io/learn/x402\n- name: trial-mode\n  type: none\n  in: query or header\n  parameter: 'trial=1 | X-2s-Trial: 1'\n  applied_to: all operations except feedback_send\n  description: 'Bypasses payment for one free real call per endpoint per hour (response marked meta.trial). Not an authentication scheme — an allowance; recorded so an agent knows the anonymous path exists. Declared as components.parameters.TrialMode.'\n  sources:\n  - openapi/2s-io-openapi.json\n  - https://2s.io/llms.txt\n- name: hosted-mcp-signer\n  type: apiKey\n  in: header\n  parameter:\
  \ X-EVM-Private-Key\n  applied_to: https://2s.io/mcp (hosted MCP server) only\n  description: >-\n    The hosted MCP server signs x402 payments on the caller's behalf, so it takes the caller's EVM private key\n    (funded with USDC on Base) as a request header. The provider's own docs warn: \"a hosted signer means your key\n    transits 2s infrastructure — for keys that never leave your machine, prefer the local SDK / npx\". Not used by\n    the REST API. initialize and tools/list need no header at all.\n  sources:\n  - https://2s.io/learn/x402/mcp\n  - mcp/2s-io-mcp.yml\ncredentials_and_secrets:\n  api_keys: none — the service issues no credentials\n  wallet_key: 'the caller''s own EVM (EVM_PRIVATE_KEY) or Solana key, held by the caller''s client; the SDKs accept a viem signer or a raw private key'\n  key_prefixes: not applicable\n  rotation: not applicable\nresponse_authenticity:\n  mechanism: 'optional response attestation — ?sign=1 adds X-2s-Attestation-* headers with an EIP-191 signature\
  \ by 0xC20d180f1d8aaf2117d13252C5E803895F0D7717 over sha256(body); the body is unchanged'\n  docs: https://2s.io/.well-known/2s-attestation.json\n  callback_signing: 'watcher / schedule / pub-sub deliveries are EIP-191-signed by the provider''s published key (X-2s-Signature)'\noauth: null\noidc: null\nmtls: null\nnotes:\n- The security scheme is declared with type apiKey because OpenAPI has no payment type; semantically it is a per-request bearer of value, not a credential. Nothing to store, rotate or leak on the 2s side.\n- No /.well-known/oauth-authorization-server, /.well-known/openid-configuration or /.well-known/oauth-protected-resource is served (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2s-io/refs/heads/main/authentication/2s-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- Public Records
- Government Data
- Finance
- Crypto
- Security
- Legal
- Weather
- Geocoding
- EDI
- AI Gateway
- Agent Infrastructure
- Webhook
- Agent-Native
---
