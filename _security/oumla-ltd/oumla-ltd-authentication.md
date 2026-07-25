---
api_key_in:
- header
api_specs:
- filename: oumla-ltd-addresses-api-openapi.yml
  format: yaml
  label: Oumla Ltd addresses API
  slug: oumla-ltd-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-addresses-api-openapi.yml
- filename: oumla-ltd-assets-api-openapi.yml
  format: yaml
  label: Oumla Ltd assets API
  slug: oumla-ltd-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-assets-api-openapi.yml
- filename: oumla-ltd-contract-interactions-api-openapi.yml
  format: yaml
  label: Oumla Ltd contract-interactions API
  slug: oumla-ltd-contract-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-contract-interactions-api-openapi.yml
- filename: oumla-ltd-contract-templates-api-openapi.yml
  format: yaml
  label: Oumla Ltd contract-templates API
  slug: oumla-ltd-contract-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-contract-templates-api-openapi.yml
- filename: oumla-ltd-deployed-contracts-api-openapi.yml
  format: yaml
  label: Oumla Ltd deployed-contracts API
  slug: oumla-ltd-deployed-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-deployed-contracts-api-openapi.yml
- filename: oumla-ltd-networks-api-openapi.yml
  format: yaml
  label: Oumla Ltd networks API
  slug: oumla-ltd-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-networks-api-openapi.yml
- filename: oumla-ltd-profiles-api-openapi.yml
  format: yaml
  label: Oumla Ltd profiles API
  slug: oumla-ltd-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-profiles-api-openapi.yml
- filename: oumla-ltd-tokenization-api-openapi.yml
  format: yaml
  label: Oumla Ltd tokenization API
  slug: oumla-ltd-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-tokenization-api-openapi.yml
- filename: oumla-ltd-transactions-api-openapi.yml
  format: yaml
  label: Oumla Ltd transactions API
  slug: oumla-ltd-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-transactions-api-openapi.yml
- filename: oumla-ltd-wallets-api-openapi.yml
  format: yaml
  label: Oumla Ltd wallets API
  slug: oumla-ltd-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-wallets-api-openapi.yml
- filename: oumla-ltd-withdraw-api-openapi.yml
  format: yaml
  label: Oumla Ltd withdraw API
  slug: oumla-ltd-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-withdraw-api-openapi.yml
- filename: oumla-ltd-workflows-api-openapi.yml
  format: yaml
  label: Oumla Ltd workflows API
  slug: oumla-ltd-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oumla Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oumla Ltd secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oumla Ltd
provider_slug: oumla-ltd
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/oumla-ltd-openapi-original.json
  type: apiKey
slug: oumla-ltd-authentication
source_filename: oumla-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oumla-ltd-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication\n  sources:\n  - openapi/oumla-ltd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/authentication/oumla-ltd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Digital Assets
- Wallet Infrastructure
- Custody
- Tokenization
- Smart Contracts
- Web3
- Fintech
- Saudi Arabia
---
