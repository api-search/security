---
api_key_in: []
api_specs:
- filename: blockstream-addresses-api-openapi.yml
  format: yaml
  label: Blockstream Addresses API
  slug: blockstream-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-addresses-api-openapi.yml
- filename: blockstream-assets-api-openapi.yml
  format: yaml
  label: Blockstream Assets API
  slug: blockstream-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-assets-api-openapi.yml
- filename: blockstream-blocks-api-openapi.yml
  format: yaml
  label: Blockstream Blocks API
  slug: blockstream-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-blocks-api-openapi.yml
- filename: blockstream-fee-estimates-api-openapi.yml
  format: yaml
  label: Blockstream Fee Estimates API
  slug: blockstream-fee-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-fee-estimates-api-openapi.yml
- filename: blockstream-mempool-api-openapi.yml
  format: yaml
  label: Blockstream Mempool API
  slug: blockstream-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-mempool-api-openapi.yml
- filename: blockstream-mining-api-openapi.yml
  format: yaml
  label: Blockstream Mining API
  slug: blockstream-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-mining-api-openapi.yml
- filename: blockstream-transactions-api-openapi.yml
  format: yaml
  label: Blockstream Transactions API
  slug: blockstream-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-transactions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Blockstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockstream declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Blockstream
provider_slug: blockstream
scheme_count: 0
schemes: []
slug: blockstream-authentication
source_filename: blockstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/Blockstream/esplora/blob/master/API.md\ndocs: https://github.com/Blockstream/esplora/blob/master/API.md\nsummary:\n  types: []\n  authentication_required: false\n  note: >-\n    The Blockstream Esplora HTTP API is a public, read-mostly block explorer API\n    that requires no authentication, API key, or OAuth token. All endpoints are\n    open. The single write path (POST /tx broadcast) is also unauthenticated;\n    network consensus rules validate the submitted transaction. There are no\n    securitySchemes declared in the OpenAPI because none are used.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/authentication/blockstream-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Bitcoin
- Blockchain
- Cryptocurrency
- Block Explorer
- Financial Services
- Infrastructure
---
