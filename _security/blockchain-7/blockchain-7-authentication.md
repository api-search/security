---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blockchain-7-bitcoin-api-openapi.yml
  format: yaml
  label: Blockchain.com Bitcoin API
  slug: blockchain-7-bitcoin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/openapi/blockchain-7-bitcoin-api-openapi.yml
- filename: blockchain-7-bitcoin-cash-api-openapi.yml
  format: yaml
  label: Blockchain.com Bitcoin Cash API
  slug: blockchain-7-bitcoin-cash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/openapi/blockchain-7-bitcoin-cash-api-openapi.yml
- filename: blockchain-7-charts-api-openapi.yml
  format: yaml
  label: Blockchain.com Charts API
  slug: blockchain-7-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/openapi/blockchain-7-charts-api-openapi.yml
- filename: blockchain-7-ethereum-api-openapi.yml
  format: yaml
  label: Blockchain.com Ethereum API
  slug: blockchain-7-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/openapi/blockchain-7-ethereum-api-openapi.yml
- filename: blockchain-7-solana-api-openapi.yml
  format: yaml
  label: Blockchain.com Solana API
  slug: blockchain-7-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/openapi/blockchain-7-solana-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blockchain 7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockchain.com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Blockchain.com
provider_slug: blockchain-7
scheme_count: 1
schemes:
- evidence: The access token should be included in resource endpoint requests as an authorization header containing a “ bearer token ”.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: blockchain-7-authentication
source_filename: blockchain-7-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.blockchain.com/oauth-resources
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.blockchain.com/oauth-resources\nsources:\n- https://docs.blockchain.com/oauth-resources\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The access token should be included in resource endpoint requests as an authorization header containing a “ bearer token ”.\n  location: header\n  header: Authorization\ndocs: https://docs.blockchain.com/oauth-resources\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain-7/refs/heads/main/authentication/blockchain-7-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Crypto
- Wallets
- Data
---
