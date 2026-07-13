---
api_key_in:
- header
api_specs:
- filename: biconomy-supertransaction-api-openapi.yml
  format: yaml
  label: Biconomy Supertransaction API
  slug: biconomy-supertransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/openapi/biconomy-supertransaction-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Biconomy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biconomy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Biconomy
provider_slug: biconomy
scheme_count: 1
schemes:
- description: 'API Key required to access Supertransaction API. Example: mee_2w3mXCuyt4xVXDRCZ5k5Lhgs'
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/biconomy-supertransaction-api-openapi.yml
  type: apiKey
slug: biconomy-authentication
source_filename: biconomy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/biconomy-supertransaction-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API Key required to access Supertransaction API. Example: mee_2w3mXCuyt4xVXDRCZ5k5Lhgs'\n  sources:\n  - openapi/biconomy-supertransaction-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/authentication/biconomy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Account Abstraction
- Blockchain
- Bundler
- Cross-Chain
- DeFi
- ERC-4337
- ERC-7579
- ERC-7702
- Ethereum
- Gas Abstraction
- Gasless
- MEE
- Paymaster
- Smart Accounts
- Smart Sessions
- Wallets
- Web3
---
