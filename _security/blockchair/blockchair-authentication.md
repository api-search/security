---
api_key_in:
- query
api_specs:
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Address Dashboards API
  slug: address-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Transaction Dashboards API
  slug: transaction-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Block Dashboards API
  slug: block-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Raw Data API
  slug: raw-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Outputs Database API
  slug: outputs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Broadcast API
  slug: broadcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blockchair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockchair secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blockchair
provider_slug: blockchair
scheme_count: 1
schemes:
- description: Optional API key passed as the `key` query parameter. Up to 1440 requests per day are allowed without a key for personal/testing use.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/blockchair-openapi.yml
  type: apiKey
slug: blockchair-authentication
source_filename: blockchair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blockchair-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Optional API key passed as the `key` query parameter. Up to 1440 requests per\n    day are allowed without a key for personal/testing use.\n  sources:\n  - openapi/blockchair-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/authentication/blockchair-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- Explorer
- Bitcoin
- Ethereum
- On-Chain Data
---
