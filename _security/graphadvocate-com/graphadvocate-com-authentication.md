---
anonymous_access: true
api_key_in: []
api_specs:
- filename: graphadvocate-com-openapi.yml
  format: yaml
  label: Graph Advocate API
  slug: graph-advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphadvocate-com/refs/heads/main/openapi/graphadvocate-com-openapi.yml
auth_types:
- none
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Graphadvocate Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaulieB14 secures its APIs with none and x402-payment across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PaulieB14
provider_slug: graphadvocate-com
scheme_count: 4
schemes:
- applies_to: POST / (A2A), POST /chat, GET /copytrade/*, GET /mcp + POST /mcp (MCP), all discovery documents
  description: Anonymous. POST /chat is free and returns the query to run (never the data). POST / over A2A is free for 3 routed queries/day when the sender is identified (below); anonymous A2A calls are charged from call 1.
  name: none
  sources:
  - quickstart
  - llms.txt
  - capabilities.json
  type: none
- applies_to: POST /route, /tip, /ask, /agent/score, /onchain-x402/address, /hyperliquid/*, /polymarket/*, /kalshi/*, /kalshi-polymarket/spread, /predmarket/spread, /narrative/divergence, /uniswap/*
  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
  challenge: HTTP 402 with `payment-required` header (base64 x402 v2 PaymentRequired) and JSON body accepts[]
  description: The client signs an EIP-3009 transferWithAuthorization for the quoted amount and retries with X-PAYMENT; the facilitator verifies and settles, then the handler runs. Over A2A the same payment can be carried by prefixing the message text with `x402:<signed-payment>` (card extension description).
  facilitator: https://api.cdp.coinbase.com/platform/v2/x402 (CDP)
  header: X-PAYMENT
  name: x402
  network: eip155:8453 (Base)
  observed:
    fetched: '2026-09-19'
    http_status: 402
    url: https://graphadvocate.com/route
  sources:
  - agent card capabilities.extensions
  - docs x402 page
  - live 402
  type: payment
- description: Not a credential. Presence of a wallet address in message metadata claims the 3/day free routing allowance; the provider notes a bare `name` no longer qualifies because rotating names minted unlimited free buckets. Nothing is verified about the address at request time; abuse is bounded by the quota.
  location: A2A request `params.metadata.sender` (or `address`) — a 42-char 0x EVM address
  name: identified-sender
  sources:
  - capabilities.json pricing.free_tier_how
  - llms.txt
  - quickstart
  type: self-asserted-identity
- applies_to: GET /quality, GET /export/stats, POST /admin/outreach-pay
  description: Operator-only endpoints require Authorization Bearer <ADMIN_TOKEN>. Not available to the public and not in the OpenAPI; recorded so no one mistakes it for a customer auth path.
  name: admin-bearer
  scheme: bearer
  sources:
  - llms.txt
  - docs x402 page
  type: http
slug: graphadvocate-com-authentication
source_filename: graphadvocate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://docs.graphadvocate.com/quickstart (\"No auth, no keys, nothing to install\"), https://graphadvocate.com/llms.txt\n  (Pricing + Identity sections), https://graphadvocate.com/agents/capabilities.json (pricing.free_tier_how), the\n  served OpenAPI (no securitySchemes, no security), the A2A card (no securitySchemes), and one live anonymous POST\n  /route (HTTP 402). derive-authentication.py produced no profile because the spec declares no securitySchemes —\n  that absence is accurate and is the finding.\ndocs: https://docs.graphadvocate.com/quickstart\nsummary:\n  types: [none, x402-payment]\n  api_key_in: []\n  oauth2_flows: []\n  signup_required: false\n  model: >-\n    Graph Advocate has NO authentication. Access is metered by payment (x402, USDC on Base) and, for the free tier,\n    by a self-asserted wallet address in the A2A message metadata. The provider states this as a design choice:\n    \"No signup, no\
  \ card, no API key — ever.\" The billing relationship is the calling agent's wallet.\nschemes:\n- name: none\n  type: none\n  applies_to: POST / (A2A), POST /chat, GET /copytrade/*, GET /mcp + POST /mcp (MCP), all discovery documents\n  description: >-\n    Anonymous. POST /chat is free and returns the query to run (never the data). POST / over A2A is free for 3\n    routed queries/day when the sender is identified (below); anonymous A2A calls are charged from call 1.\n  sources: [quickstart, llms.txt, capabilities.json]\n- name: x402\n  type: payment\n  header: X-PAYMENT\n  challenge: HTTP 402 with `payment-required` header (base64 x402 v2 PaymentRequired) and JSON body accepts[]\n  network: 'eip155:8453 (Base)'\n  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n  facilitator: https://api.cdp.coinbase.com/platform/v2/x402 (CDP)\n  applies_to: POST /route, /tip, /ask, /agent/score, /onchain-x402/address, /hyperliquid/*, /polymarket/*, /kalshi/*, /kalshi-polymarket/spread, /predmarket/spread,\
  \ /narrative/divergence, /uniswap/*\n  description: >-\n    The client signs an EIP-3009 transferWithAuthorization for the quoted amount and retries with X-PAYMENT; the\n    facilitator verifies and settles, then the handler runs. Over A2A the same payment can be carried by prefixing\n    the message text with `x402:<signed-payment>` (card extension description).\n  observed: {url: https://graphadvocate.com/route, http_status: 402, fetched: '2026-09-19'}\n  sources: [agent card capabilities.extensions, docs x402 page, live 402]\n- name: identified-sender\n  type: self-asserted-identity\n  location: A2A request `params.metadata.sender` (or `address`) — a 42-char 0x EVM address\n  description: >-\n    Not a credential. Presence of a wallet address in message metadata claims the 3/day free routing allowance;\n    the provider notes a bare `name` no longer qualifies because rotating names minted unlimited free buckets.\n    Nothing is verified about the address at request time; abuse is bounded\
  \ by the quota.\n  sources: [capabilities.json pricing.free_tier_how, llms.txt, quickstart]\n- name: admin-bearer\n  type: http\n  scheme: bearer\n  applies_to: GET /quality, GET /export/stats, POST /admin/outreach-pay\n  description: Operator-only endpoints require Authorization Bearer <ADMIN_TOKEN>. Not available to the public and not in the OpenAPI; recorded so no one mistakes it for a customer auth path.\n  sources: [llms.txt, docs x402 page]\ndownstream_keys_the_router_hands_you:\n  note: >-\n    Responses often include a curl for The Graph gateway; running THAT needs the caller's own free Graph API key\n    (thegraph.com/studio, 100K queries/month) or Token API JWT (thegraph.market). Those are third-party\n    credentials for The Graph, not Graph Advocate credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphadvocate-com/refs/heads/main/authentication/graphadvocate-com-authentication.yml
summary_line: none/x402-payment · 4 schemes
tags:
- Blockchain
- On-Chain Data
- The Graph
- Subgraph
- GraphQL
- MCP
- A2A
- x402
- Agentic Commerce
- AI Agents
- DeFi
- Prediction Markets
- Trader Intelligence
- Web3
---
