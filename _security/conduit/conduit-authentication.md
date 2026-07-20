---
api_key_in:
- path
api_specs:
- filename: conduit-nodes-openapi.json
  format: json
  label: Conduit Nodes
  slug: conduit-nodes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduit/refs/heads/main/openapi/conduit-nodes-openapi.json
auth_types:
- apiKey
- mpp-payment-channel
description: ''
kind: authentication
layout: security
method: searched
name: Conduit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conduit secures its APIs with apiKey and mpp-payment-channel across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conduit
provider_slug: conduit
scheme_count: 2
schemes:
- create_url: https://app.conduit.xyz/rpc-keys
  description: RPC access is authenticated with an API key created at https://app.conduit.xyz/nodes. The key is appended to the RPC URL of the target rollup (path segment), e.g. https://rpc.<chain>.conduit.xyz/<API_KEY>. A single key works across all public and private endpoints scoped to it. Keys can be restricted by domain, IP, and contract-deployer address, and can be regenerated or deleted.
  in: path
  name: rpcApiKey
  restrictions:
  - domain
  - ip-address
  - contract-deployer-address
  scoping: per-network (a key scoped to one network returns -32403 "unauthorized rpc key" on another)
  type: apiKey
- description: 'The agentic gateway at https://mpp.conduit.xyz authenticates via Machine Payments Protocol (MPP) sessions instead of API keys. The client opens a USDC payment channel on Tempo and sends signed off-chain vouchers with each request. First unpaid request returns 402 Payment Required with a ''WWW-Authenticate: Payment'' header. Cost is $0.00005 per JSON-RPC call.'
  docs: https://docs.conduit.xyz/rpc-nodes/getting-started/agent-skills
  gateway: https://mpp.conduit.xyz
  name: mppSession
  scheme: payment-channel
  type: http
slug: conduit-authentication
source_filename: conduit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.conduit.xyz/rpc-nodes/getting-started/get-api-key.md\ndocs: https://docs.conduit.xyz/rpc-nodes/getting-started/get-api-key\n# The published OpenAPI (openapi/conduit-nodes-openapi.json) declares no\n# securitySchemes, so this profile is captured from the docs, not derived.\nsummary:\n  types: [apiKey, mpp-payment-channel]\n  api_key_in: [path]\n  oauth2_flows: []\nschemes:\n- name: rpcApiKey\n  type: apiKey\n  in: path\n  description: >-\n    RPC access is authenticated with an API key created at\n    https://app.conduit.xyz/nodes. The key is appended to the RPC URL of the\n    target rollup (path segment), e.g.\n    https://rpc.<chain>.conduit.xyz/<API_KEY>. A single key works across all\n    public and private endpoints scoped to it. Keys can be restricted by domain,\n    IP, and contract-deployer address, and can be regenerated or deleted.\n  create_url: https://app.conduit.xyz/rpc-keys\n  scoping: per-network\
  \ (a key scoped to one network returns -32403 \"unauthorized\n    rpc key\" on another)\n  restrictions: [domain, ip-address, contract-deployer-address]\n- name: mppSession\n  type: http\n  scheme: payment-channel\n  description: >-\n    The agentic gateway at https://mpp.conduit.xyz authenticates via Machine\n    Payments Protocol (MPP) sessions instead of API keys. The client opens a\n    USDC payment channel on Tempo and sends signed off-chain vouchers with each\n    request. First unpaid request returns 402 Payment Required with a\n    'WWW-Authenticate: Payment' header. Cost is $0.00005 per JSON-RPC call.\n  gateway: https://mpp.conduit.xyz\n  docs: https://docs.conduit.xyz/rpc-nodes/getting-started/agent-skills\nunauthenticated_access:\n  allowed: true\n  note: Public RPC endpoints are usable without a key at a reduced 200 CU/s throughput tier.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conduit/refs/heads/main/authentication/conduit-authentication.yml
summary_line: apiKey/mpp-payment-channel · 2 schemes
tags:
- Company
- Crypto Infrastructure
- Blockchain
- Rollups
- RPC Nodes
- Web3
- Ethereum
- Node Infrastructure
---
