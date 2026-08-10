---
api_key_in: []
api_specs:
- filename: bykaranteli-x402-api-openapi.yml
  format: yaml
  label: ByKaranteli X402 API
  slug: bykaranteli-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/openapi/bykaranteli-x402-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Bykaranteli Authentication
name_suffix: Authentication
oauth_flows: []
overview: ByKaranteli declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: ByKaranteli
provider_slug: bykaranteli
scheme_count: 4
schemes:
- applies_to:
  - /api/public/*
  - /api/v1/public/* (except /me)
  - /api/liqmap/public
  - /embed/*
  - /feed.xml
  description: No authentication. CORS Access-Control-Allow-Origin is *, GET and OPTIONS preflight are supported, responses are read-only and carry no PII.
  evidence: developers page "Auth · None · All endpoints public / read-only"
  id: none
  type: none
- alternatives:
  - query parameter ?api_key= (for clients that cannot set headers, e.g. calendar feeds)
  - query parameter ?token=
  applies_to:
  - /api/v1/public/me
  - /api/v1/me/*
  description: Member-scoped Bearer token. Same response shape as /api/v1/public/profiles/[handle] but for the key owner.
  evidence: '/api/v1/public/manifest -> conventions.auth: "Bearer token in Authorization header, or ?api_key= / ?token= for clients that can''t set headers."'
  format: 'Authorization: Bearer <api key>'
  header: Authorization
  id: bearer_api_key
  in: header
  rate_limit: 60 req/min/key
  requires: member account with public_profile_enabled
  scheme: bearer
  type: http
- applies_to:
  - /api/x402/* (13 paid endpoints; /api/x402 catalog itself is free)
  assets:
  - USDC
  challenge_header: payment-required
  challenge_status: 402
  description: Call the endpoint with no payment and it answers HTTP 402 with a base64 `payment-required` header carrying x402 v2 payment requirements — resource URL, service name, tags, accepted networks/assets/amounts, and a `bazaar` extension whose JSON Schema describes the call's input and output shape. An x402 client pays and retries automatically. Price is per SUCCESSFUL response; a failed request settles nothing. No signup on either side.
  evidence:
    fetched: '2026-08-09'
    http_status: 402
    url: https://bykaranteli.com/api/x402/flow-vpin
  id: x402_payment
  in: header
  max_timeout_seconds: 300
  networks:
  - asset_mint: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v
    chain: Solana mainnet
    fee_payer: GVJJ7rdGiXr5xaYbRwRbjfaJL7fmwRygFi1H6aGqDveb
    id: solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp
    pay_to: 4JgPtoBWkQyG3QffVJC3bfgk7SCQrz9bx2SAEUTSVqzK
  - asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    chain: Base mainnet
    id: eip155:8453
    pay_to: '0x0db4c96d8b14f431f3bb8ce1a33f07d2c696a62c'
  protocol: x402
  request_header: X-PAYMENT
  scheme: exact
  type: payment
  verbatim_challenge: examples/bykaranteli-x402-payment-required.json
  version: 2
- applies_to:
  - https://mcp.bykaranteli.com (Streamable HTTP)
  description: Hosted MCP server requires no key. No OAuth discovery documents are published (/.well-known/oauth-authorization-server and /oauth-protected-resource both 404), consistent with an unauthenticated read-only server.
  evidence:
    http_status: 200
    method: POST tools/list
    result: 20 tools returned anonymously
    url: https://mcp.bykaranteli.com
  id: mcp_anonymous
  type: none
slug: bykaranteli-authentication
source_filename: bykaranteli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://bykaranteli.com/developers\ndocs: https://bykaranteli.com/developers\nalso_searched:\n  - https://bykaranteli.com/api/v1/public/manifest\n  - https://bykaranteli.com/openapi.json\n  - https://mcp.bykaranteli.com\n\nsummary: >-\n  ByKaranteli runs three distinct access models on one host. The public read\n  surface (/api/public/*, /api/v1/public/*) takes no credential at all. A small\n  account surface (/api/v1/public/me, /api/v1/me/*) takes a Bearer API key owned\n  by a registered member. The paid agent surface (/api/x402/*) takes no account\n  and no key — it authenticates the CALL, not the caller, by settling a USDC\n  micropayment over the x402 protocol. The hosted MCP server at\n  mcp.bykaranteli.com answered an anonymous tools/list, confirming it is\n  unauthenticated.\n\nschemes:\n  - id: none\n    type: none\n    applies_to:\n      - /api/public/*\n      - /api/v1/public/* (except /me)\n      - /api/liqmap/public\n\
  \      - /embed/*\n      - /feed.xml\n    description: >-\n      No authentication. CORS Access-Control-Allow-Origin is *, GET and OPTIONS\n      preflight are supported, responses are read-only and carry no PII.\n    evidence: 'developers page \"Auth · None · All endpoints public / read-only\"'\n\n  - id: bearer_api_key\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <api key>'\n    alternatives:\n      - 'query parameter ?api_key= (for clients that cannot set headers, e.g. calendar feeds)'\n      - 'query parameter ?token='\n    applies_to:\n      - /api/v1/public/me\n      - /api/v1/me/*\n    requires: member account with public_profile_enabled\n    rate_limit: 60 req/min/key\n    description: >-\n      Member-scoped Bearer token. Same response shape as\n      /api/v1/public/profiles/[handle] but for the key owner.\n    evidence: >-\n      /api/v1/public/manifest -> conventions.auth: \"Bearer token in Authorization\n\
  \      header, or ?api_key= / ?token= for clients that can't set headers.\"\n\n  - id: x402_payment\n    type: payment\n    protocol: x402\n    version: 2\n    in: header\n    request_header: X-PAYMENT\n    challenge_header: payment-required\n    challenge_status: 402\n    applies_to:\n      - /api/x402/* (13 paid endpoints; /api/x402 catalog itself is free)\n    assets: [USDC]\n    networks:\n      - id: 'solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp'\n        chain: Solana mainnet\n        asset_mint: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v\n        pay_to: 4JgPtoBWkQyG3QffVJC3bfgk7SCQrz9bx2SAEUTSVqzK\n        fee_payer: GVJJ7rdGiXr5xaYbRwRbjfaJL7fmwRygFi1H6aGqDveb\n      - id: 'eip155:8453'\n        chain: Base mainnet\n        asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n        pay_to: '0x0db4c96d8b14f431f3bb8ce1a33f07d2c696a62c'\n    scheme: exact\n    max_timeout_seconds: 300\n    description: >-\n      Call the endpoint with no payment and it answers HTTP 402 with\
  \ a base64\n      `payment-required` header carrying x402 v2 payment requirements — resource\n      URL, service name, tags, accepted networks/assets/amounts, and a `bazaar`\n      extension whose JSON Schema describes the call's input and output shape.\n      An x402 client pays and retries automatically. Price is per SUCCESSFUL\n      response; a failed request settles nothing. No signup on either side.\n    verbatim_challenge: examples/bykaranteli-x402-payment-required.json\n    evidence:\n      url: https://bykaranteli.com/api/x402/flow-vpin\n      http_status: 402\n      fetched: '2026-08-09'\n\n  - id: mcp_anonymous\n    type: none\n    applies_to:\n      - https://mcp.bykaranteli.com (Streamable HTTP)\n    description: >-\n      Hosted MCP server requires no key. No OAuth discovery documents are\n      published (/.well-known/oauth-authorization-server and\n      /oauth-protected-resource both 404), consistent with an unauthenticated\n      read-only server.\n    evidence:\n   \
  \   url: https://mcp.bykaranteli.com\n      method: 'POST tools/list'\n      http_status: 200\n      result: 20 tools returned anonymously\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: none\nnotes:\n  - >-\n    There is no OAuth surface, so no scopes/ artifact is emitted — the key-auth\n    member surface carries the model instead.\n  - >-\n    The published OpenAPI (/openapi.json) declares no components.securitySchemes;\n    it marks the free catalog operation `security: []` and leaves the paid\n    operations implicitly gated by the 402 flow. That is the one authentication\n    gap worth raising with the provider — an `x-payment-info` extension is\n    present per operation, but a formal securityScheme is not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/authentication/bykaranteli-authentication.yml
summary_line: 4 schemes
tags:
- Cryptocurrency
- Crypto Derivatives
- Market Data
- Funding Rates
- Open Interest
- Liquidations
- Options
- ETF Flows
- Financial Data
- MCP
- x402
- Agents
---
