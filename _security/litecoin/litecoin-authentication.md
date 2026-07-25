---
api_key_in: []
api_specs:
- filename: litecoin-addresses-api-openapi.yml
  format: yaml
  label: Litecoin Addresses API
  slug: litecoin-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-addresses-api-openapi.yml
- filename: litecoin-blockchain-api-openapi.yml
  format: yaml
  label: Litecoin Blockchain API
  slug: litecoin-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-blockchain-api-openapi.yml
- filename: litecoin-blocks-api-openapi.yml
  format: yaml
  label: Litecoin Blocks API
  slug: litecoin-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-blocks-api-openapi.yml
- filename: litecoin-fees-api-openapi.yml
  format: yaml
  label: Litecoin Fees API
  slug: litecoin-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-fees-api-openapi.yml
- filename: litecoin-json-rpc-api-openapi.yml
  format: yaml
  label: Litecoin JSON-RPC API
  slug: litecoin-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-json-rpc-api-openapi.yml
- filename: litecoin-mempool-api-openapi.yml
  format: yaml
  label: Litecoin Mempool API
  slug: litecoin-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-mempool-api-openapi.yml
- filename: litecoin-mining-api-openapi.yml
  format: yaml
  label: Litecoin Mining API
  slug: litecoin-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-mining-api-openapi.yml
- filename: litecoin-transactions-api-openapi.yml
  format: yaml
  label: Litecoin Transactions API
  slug: litecoin-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-transactions-api-openapi.yml
- filename: litecoin-utxo-api-openapi.yml
  format: yaml
  label: Litecoin UTXO API
  slug: litecoin-utxo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-utxo-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Litecoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Litecoin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Litecoin
provider_slug: litecoin
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using credentials from the .litecoin/.cookie file or configured via rpcauth in litecoin.conf.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/litecoin-core-json-rpc.yml
  type: http
slug: litecoin-authentication
source_filename: litecoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/litecoin-core-json-rpc.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using credentials from the .litecoin/.cookie file or\n    configured via rpcauth in litecoin.conf.\n  sources:\n  - openapi/litecoin-core-json-rpc.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/authentication/litecoin-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- Blockchain
- Litecoin
- LTC
- Payments
- Decentralized Finance
- Block Explorer
- JSON-RPC
---
