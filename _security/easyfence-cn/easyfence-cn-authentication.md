---
anonymous_access: true
api_key_in: []
api_specs:
- filename: easyfence-cn-store-api-openapi.yml
  format: yaml
  label: X402 AI 自助门店 Store API
  slug: easyfence-cn-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyfence-cn/refs/heads/main/openapi/easyfence-cn-store-api-openapi.yml
- filename: easyfence-cn-facilitator-api-openapi.yml
  format: yaml
  label: X402 AI 自助门店 x402 Facilitator API
  slug: easyfence-cn-x402-facilitator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyfence-cn/refs/heads/main/openapi/easyfence-cn-facilitator-api-openapi.yml
auth_types:
- none
- x402-payment
- erc8004-identity
- query-token
description: 'The provider''s OpenAPI declares NO securitySchemes and no security requirement on any operation, so derive-authentication.py produced nothing. The real access model is not HTTP authentication at all: the public surface is anonymous, the paid surface is gated by an x402 payment (HTTP 402 with a payment requirement, satisfied by an EIP-3009 USDC transfer authorization), identity is an ERC-8004 style card verified out-of-band, and the operator console is gated by a shared token in a query string. Every entry below was observed live on 2026-09-19.'
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Easyfence Cn Authentication
name_suffix: Authentication
oauth_flows: []
overview: X402 AI 自助门店 secures its APIs with none, x402-payment, erc8004-identity, and query-token across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: X402 AI 自助门店
provider_slug: easyfence-cn
scheme_count: 4
schemes:
- description: No credential of any kind. The catalog, the trust registry, both health endpoints, the agent card and the A2A JSON-RPC endpoint all answered without headers. The agent card declares no securitySchemes and no security, so an A2A client will read the agent as unauthenticated.
  name: anonymous
  probes:
  - method: GET
    status: 200
    url: https://www.easyfence.cn/api/catalog
  - method: GET
    status: 200
    url: https://www.easyfence.cn/api/registry
  - body: '{"ok":false,"reason":"字段缺失"}'
    method: POST {}
    note: reachable anonymously; answered "fields missing"
    status: 200
    url: https://www.easyfence.cn/api/identity/verify
  - body: JSON-RPC -32601
    method: POST tasks/get
    status: 400
    url: https://www.easyfence.cn/a2a
  surface: GET /api/catalog, GET /api/registry, GET /healthz, GET /facilitator/healthz, GET /.well-known/agent.json, POST /api/identity/verify, POST /a2a
  type: none
- description: 'The delivery endpoint answers HTTP 402 Payment Required with an x402 payment-requirements body until the buyer presents a signed payment. accepts[] offers two routes for the same 0.50 USD service: scheme "exact" on network base (chainId 8453, asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 = USDC, maxAmountRequired 500000 = 0.50 USDC at 6 decimals, facilitator https://x402.org/facilitator) and scheme "exact" on network bsc (chainId 56, asset 0x8AC76a51cc950d9822D68b83fE1Ad97B32Cd580d, maxAmountRequired 500000000000000000 = 0.50 at 18 decimals, facilitator https://www.easyfence.cn/facilitator). Both pay to 0xF9E7138dDC630EFa202B56bBDca42466F5F25B93 with maxTimeoutSeconds 60. The /a2a explainer says the buyer signs an EIP-3009 authorization and retries. /healthz reports payment_mode "mainnet-real": this is live money, not a sandbox. The Base route also carries an x402 "bazaar" extension with an input JSON Schema for the request body (service, params.brief, optional buyer_agent).'
  name: x402
  probes:
  - content_type: application/json
    headers: 'accept: exact'
    method: POST {"service":"write_script","params":{"brief":"probe"}}
    note: full x402 payment-requirements body returned; no payment was made
    status: 402
    url: https://www.easyfence.cn/api/deliver
  - body: '{"error":"未知服务","known":[...7 ids]}'
    method: POST {}
    note: an unknown service is rejected BEFORE the payment gate
    status: 400
    url: https://www.easyfence.cn/api/deliver
  scheme: x402 exact (x402Version 1)
  surface: POST /api/deliver
  type: payment
- description: 'The card''s auth.identity is "erc8004" and the home page describes step two of a sale as the buyer presenting an ERC-8004 on-chain identity card that the store verifies. /api/identity/verify accepts a presented card and answers {ok, reason}; /api/identity/issue (marked demo in its own description) signs a card for an agent address with the store issuer key; /api/registry publishes the issuer (0x63D4b01ecba21a15c324559dd324928fe57b3Bbe) and trusted_issuers (currently the same address) with count 0 agents. Identity is presented as data, not as an HTTP credential, and nothing observed requires it: the 402 challenge was returned to an unidentified caller.'
  name: erc8004
  probes:
  - body: '{"registry":"X402 ERC-8004 Trust Registry","issuer":"0x63D4...3Bbe","trusted_issuers":[...],"count":0,"agents":[]}'
    method: GET
    status: 200
    url: https://www.easyfence.cn/api/registry
  scheme: ERC-8004 style identity card, EIP-712 signed
  surface: POST /api/identity/verify, POST /api/identity/issue, GET /api/registry
  type: identity
- description: The operator console answers 401 with an HTML hint "访问 /admin?token=你的ADMIN_TOKEN" (visit /admin?token=YOUR_ADMIN_TOKEN). A single shared secret in the query string; not a public developer credential and not probed further.
  in: query
  name: adminToken
  name_param: token
  probes:
  - content_type: text/html
    method: GET
    status: 401
    url: https://www.easyfence.cn/admin
  surface: GET /admin, GET|POST /admin/config, GET /admin/revenue, GET|POST /admin/services
  type: apiKey
slug: easyfence-cn-authentication
source_filename: easyfence-cn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource:\n- https://www.easyfence.cn/openapi.json\n- https://www.easyfence.cn/.well-known/agent.json\n- https://www.easyfence.cn/api/deliver (POST, live 402 challenge)\n- https://www.easyfence.cn/a2a (GET explainer page)\n- https://www.easyfence.cn/admin\ndocs: https://www.easyfence.cn/a2a\nspec: openapi/easyfence-cn-store-api-openapi.yml\ndescription: >-\n  The provider's OpenAPI declares NO securitySchemes and no security requirement on any operation, so\n  derive-authentication.py produced nothing. The real access model is not HTTP authentication at all: the\n  public surface is anonymous, the paid surface is gated by an x402 payment (HTTP 402 with a payment\n  requirement, satisfied by an EIP-3009 USDC transfer authorization), identity is an ERC-8004 style card\n  verified out-of-band, and the operator console is gated by a shared token in a query string. Every\n  entry below was observed live on 2026-09-19.\nsummary:\n  types: [none,\
  \ x402-payment, erc8004-identity, query-token]\n  transport: HTTPS; the payment authorization travels in the retried request per the x402 protocol\nschemes:\n- name: anonymous\n  type: none\n  surface: >-\n    GET /api/catalog, GET /api/registry, GET /healthz, GET /facilitator/healthz, GET /.well-known/agent.json,\n    POST /api/identity/verify, POST /a2a\n  description: >-\n    No credential of any kind. The catalog, the trust registry, both health endpoints, the agent card and\n    the A2A JSON-RPC endpoint all answered without headers. The agent card declares no securitySchemes and\n    no security, so an A2A client will read the agent as unauthenticated.\n  probes:\n  - {url: 'https://www.easyfence.cn/api/catalog', method: GET, status: 200}\n  - {url: 'https://www.easyfence.cn/api/registry', method: GET, status: 200}\n  - {url: 'https://www.easyfence.cn/api/identity/verify', method: 'POST {}', status: 200, body: '{\"ok\":false,\"reason\":\"字段缺失\"}', note: reachable anonymously; answered\
  \ \"fields missing\"}\n  - {url: 'https://www.easyfence.cn/a2a', method: POST tasks/get, status: 400, body: JSON-RPC -32601}\n- name: x402\n  type: payment\n  scheme: x402 exact (x402Version 1)\n  surface: POST /api/deliver\n  description: >-\n    The delivery endpoint answers HTTP 402 Payment Required with an x402 payment-requirements body until\n    the buyer presents a signed payment. accepts[] offers two routes for the same 0.50 USD service:\n    scheme \"exact\" on network base (chainId 8453, asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 = USDC,\n    maxAmountRequired 500000 = 0.50 USDC at 6 decimals, facilitator https://x402.org/facilitator) and\n    scheme \"exact\" on network bsc (chainId 56, asset 0x8AC76a51cc950d9822D68b83fE1Ad97B32Cd580d,\n    maxAmountRequired 500000000000000000 = 0.50 at 18 decimals, facilitator https://www.easyfence.cn/facilitator).\n    Both pay to 0xF9E7138dDC630EFa202B56bBDca42466F5F25B93 with maxTimeoutSeconds 60. The /a2a explainer says\n    the buyer\
  \ signs an EIP-3009 authorization and retries. /healthz reports payment_mode \"mainnet-real\":\n    this is live money, not a sandbox. The Base route also carries an x402 \"bazaar\" extension with an input\n    JSON Schema for the request body (service, params.brief, optional buyer_agent).\n  probes:\n  - {url: 'https://www.easyfence.cn/api/deliver', method: 'POST {\"service\":\"write_script\",\"params\":{\"brief\":\"probe\"}}', status: 402, content_type: application/json, headers: 'accept: exact', note: full x402 payment-requirements body returned; no payment was made}\n  - {url: 'https://www.easyfence.cn/api/deliver', method: 'POST {}', status: 400, body: '{\"error\":\"未知服务\",\"known\":[...7 ids]}', note: an unknown service is rejected BEFORE the payment gate}\n- name: erc8004\n  type: identity\n  scheme: ERC-8004 style identity card, EIP-712 signed\n  surface: POST /api/identity/verify, POST /api/identity/issue, GET /api/registry\n  description: >-\n    The card's auth.identity is \"\
  erc8004\" and the home page describes step two of a sale as the buyer\n    presenting an ERC-8004 on-chain identity card that the store verifies. /api/identity/verify accepts a\n    presented card and answers {ok, reason}; /api/identity/issue (marked demo in its own description) signs\n    a card for an agent address with the store issuer key; /api/registry publishes the issuer\n    (0x63D4b01ecba21a15c324559dd324928fe57b3Bbe) and trusted_issuers (currently the same address) with\n    count 0 agents. Identity is presented as data, not as an HTTP credential, and nothing observed\n    requires it: the 402 challenge was returned to an unidentified caller.\n  probes:\n  - {url: 'https://www.easyfence.cn/api/registry', method: GET, status: 200, body: '{\"registry\":\"X402 ERC-8004 Trust Registry\",\"issuer\":\"0x63D4...3Bbe\",\"trusted_issuers\":[...],\"count\":0,\"agents\":[]}'}\n- name: adminToken\n  type: apiKey\n  in: query\n  name_param: token\n  surface: GET /admin, GET|POST /admin/config,\
  \ GET /admin/revenue, GET|POST /admin/services\n  description: >-\n    The operator console answers 401 with an HTML hint \"访问 /admin?token=你的ADMIN_TOKEN\" (visit\n    /admin?token=YOUR_ADMIN_TOKEN). A single shared secret in the query string; not a public developer\n    credential and not probed further.\n  probes:\n  - {url: 'https://www.easyfence.cn/admin', method: GET, status: 401, content_type: text/html}\noauth: false\nopenid_connect: false\napi_keys: false\nnotes: >-\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and\n  /.well-known/openid-configuration all 404 on both hosts. No scopes/ artifact is written because there\n  is no scope surface. The spec's silence on security is itself a finding: an agent reading the OpenAPI\n  alone cannot learn that /api/deliver costs money until it receives the 402.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyfence-cn/refs/heads/main/authentication/easyfence-cn-authentication.yml
summary_line: none/x402-payment/erc8004-identity/query-token · 4 schemes
tags:
- Agentic Commerce
- AI Agents
- A2A
- x402
- Payments
- Stablecoins
- Agent Identity
- Content Generation
- Web3
---
