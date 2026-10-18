---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: venice-ai-api-keys-api-openapi.yml
  format: yaml
  label: Venice.ai API Keys API
  slug: venice-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-api-keys-api-openapi.yml
- filename: venice-ai-audio-api-openapi.yml
  format: yaml
  label: Venice.ai Audio API
  slug: venice-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-audio-api-openapi.yml
- filename: venice-ai-augment-api-openapi.yml
  format: yaml
  label: Venice.ai Augment API
  slug: venice-ai-augment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-augment-api-openapi.yml
- filename: venice-ai-billing-api-openapi.yml
  format: yaml
  label: Venice.ai Billing API
  slug: venice-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-billing-api-openapi.yml
- filename: venice-ai-characters-api-openapi.yml
  format: yaml
  label: Venice.ai Characters API
  slug: venice-ai-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-characters-api-openapi.yml
- filename: venice-ai-crypto-rpc-api-openapi.yml
  format: yaml
  label: Venice.ai Crypto RPC API
  slug: venice-ai-crypto-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-crypto-rpc-api-openapi.yml
- filename: venice-ai-decisions-api-openapi.yml
  format: yaml
  label: Venice.ai Decisions API
  slug: venice-ai-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-decisions-api-openapi.yml
- filename: venice-ai-embeddings-api-openapi.yml
  format: yaml
  label: Venice.ai Embeddings API
  slug: venice-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-embeddings-api-openapi.yml
- filename: venice-ai-image-api-openapi.yml
  format: yaml
  label: Venice.ai Image API
  slug: venice-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-image-api-openapi.yml
- filename: venice-ai-models-api-openapi.yml
  format: yaml
  label: Venice.ai Models API
  slug: venice-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-models-api-openapi.yml
- filename: venice-ai-preview-api-openapi.yml
  format: yaml
  label: Venice.ai Preview API
  slug: venice-ai-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-preview-api-openapi.yml
- filename: venice-ai-responses-api-openapi.yml
  format: yaml
  label: Venice.ai Responses API
  slug: venice-ai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-responses-api-openapi.yml
- filename: venice-ai-speech-api-openapi.yml
  format: yaml
  label: Venice.ai Speech API
  slug: venice-ai-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-speech-api-openapi.yml
- filename: venice-ai-transcriptions-api-openapi.yml
  format: yaml
  label: Venice.ai Transcriptions API
  slug: venice-ai-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-transcriptions-api-openapi.yml
- filename: venice-ai-video-api-openapi.yml
  format: yaml
  label: Venice.ai Video API
  slug: venice-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-video-api-openapi.yml
- filename: venice-ai-voices-api-openapi.yml
  format: yaml
  label: Venice.ai Voices API
  slug: venice-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-voices-api-openapi.yml
- filename: venice-ai-x402-api-openapi.yml
  format: yaml
  label: Venice.ai X402 API
  slug: venice-ai-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-x402-api-openapi.yml
- filename: venice-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Venice.ai Chat Completions API
  slug: venice-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-chat-completions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Venice Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Venice.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Venice.ai
provider_slug: venice-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/venice-ai-openapi.yml
  type: http
- description: 'Wallet-based authentication using the x402 protocol (Sign-In-With-X). Supports EVM SIWE signatures on Base and Ed25519 signatures on Solana mainnet.


    **Header format:** Base64-encoded JSON object with the following fields:

    - `address` — EVM or Solana wallet address

    - `message` — Signed SIWX message. EVM wallets use EIP-4361 SIWE; Solana wallets use the Solana SIWX message format.

    - `signature` — S'
  in: header
  name: siwx
  parameter: SIGN-IN-WITH-X
  sources:
  - openapi/venice-ai-openapi.yml
  type: apiKey
slug: venice-ai-authentication
source_filename: venice-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/venice-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/venice-ai-openapi.yml\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: SIGN-IN-WITH-X\n  description: |-\n    Wallet-based authentication using the x402 protocol (Sign-In-With-X). Supports EVM SIWE signatures on Base and Ed25519 signatures on Solana mainnet.\n\n    **Header format:** Base64-encoded JSON object with the following fields:\n    - `address` — EVM or Solana wallet address\n    - `message` — Signed SIWX message. EVM wallets use EIP-4361 SIWE; Solana wallets use the Solana SIWX message format.\n    - `signature` — S\n  sources:\n  - openapi/venice-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/authentication/venice-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- Image Generation
- Video Generation
- Text-to-Speech
- Embeddings
- Privacy
- OpenAI-Compatible
- x402
---
