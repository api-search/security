---
api_key_in: []
api_specs:
- filename: litecoin-core-json-rpc.yml
  format: yaml
  label: Litecoin Core JSON-RPC API
  slug: litecoin-core-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-core-json-rpc.yml
- filename: litecoin-core-rest.yml
  format: yaml
  label: Litecoin Core REST API
  slug: litecoin-core-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-core-rest.yml
- filename: litecoin-space-rest.yml
  format: yaml
  label: Litecoin Space REST API
  slug: litecoin-space-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-space-rest.yml
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
