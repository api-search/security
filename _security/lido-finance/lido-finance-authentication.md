---
api_key_in: []
api_specs:
- filename: lido-finance-eth-api-openapi-original.json
  format: json
  label: Lido Ethereum API
  slug: lido-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-eth-api-openapi-original.json
- filename: lido-finance-withdrawal-queue-openapi-original.json
  format: json
  label: Lido Withdrawals API
  slug: lido-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-withdrawal-queue-openapi-original.json
- filename: lido-finance-reward-history-openapi-original.json
  format: json
  label: Lido Reward History Backend API
  slug: lido-reward-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-reward-history-openapi-original.json
auth_types: []
description: Lido's three public REST APIs declare no securitySchemes in their OpenAPI documents and the docs state plainly that "Lido APIs are strictly for read-only access". There are no API keys, no OAuth flows, and no scope surface. The only credentialed surface in the Lido developer stack is The Graph gateway API key required to query the Lido subgraph — that key is issued by The Graph, not by Lido.
kind: authentication
layout: security
method: searched
name: Lido Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lido Finance declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lido Finance
provider_slug: lido-finance
scheme_count: 0
schemes: []
slug: lido-finance-authentication
source_filename: lido-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.lido.fi/integrations/api\ndocs: https://docs.lido.fi/integrations/api\ndescription: >-\n  Lido's three public REST APIs declare no securitySchemes in their OpenAPI documents and the docs\n  state plainly that \"Lido APIs are strictly for read-only access\". There are no API keys, no OAuth\n  flows, and no scope surface. The only credentialed surface in the Lido developer stack is The\n  Graph gateway API key required to query the Lido subgraph — that key is issued by The Graph, not\n  by Lido.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  anonymous: true\nschemes: []\napis:\n- api: Lido Ethereum API\n  base_url: https://eth-api.lido.fi\n  auth: none\n  note: Public, unauthenticated, read-only. No securitySchemes in openapi/lido-finance-eth-api-openapi-original.json.\n- api: Lido Withdrawals API\n  base_url: https://wq-api.lido.fi\n  auth: none\n  note: >-\n    Public, unauthenticated, read-only.\
  \ An optional WQ-Request-Source header (widget | sdk | unknown)\n    is accepted for attribution, not authentication.\n- api: Lido Reward History Backend API\n  base_url: https://reward-history-backend.lido.fi\n  auth: none\n  note: Public, unauthenticated, read-only. Callers pass the subject address as a query parameter.\n- api: Lido Subgraph (GraphQL)\n  base_url: https://gateway-arbitrum.network.thegraph.com\n  auth: third-party-api-key\n  note: >-\n    Requires a The Graph Decentralized Network API key embedded in the gateway URL path\n    (/api/[api-key]/subgraphs/id/...). Issued and billed by The Graph, not by Lido.\nrelated:\n  conventions: conventions/lido-finance-conventions.yml\n  domain_security: security/lido-finance-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/authentication/lido-finance-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Blockchain
- Ethereum
- Liquid Staking
- DeFi
- Cryptocurrency
- Staking
- Web3
- Financial Services
- GraphQL
---
