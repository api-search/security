---
api_key_in:
- header
api_specs:
- filename: ava-labs-data-api-openapi.yml
  format: yaml
  label: AvaCloud Data API
  slug: avacloud-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-data-api-openapi.yml
- filename: ava-labs-metrics-api-openapi.yml
  format: yaml
  label: AvaCloud Metrics API
  slug: avacloud-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-metrics-api-openapi.yml
- filename: ava-labs-platform-api-openapi.yml
  format: yaml
  label: Avalanche Platform Chain API
  slug: avalanche-platform-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-platform-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ava Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ava Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ava Labs
provider_slug: ava-labs
scheme_count: 1
schemes:
- description: Api keys provide higher access to rate limits. To obtain an api key, sign up for an account at https://avacloud.io/.
  in: header
  name: apiKey
  parameter: x-glacier-api-key
  sources:
  - openapi/ava-labs-data-api-openapi.yml
  type: apiKey
slug: ava-labs-authentication
source_filename: ava-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/ava-labs-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-glacier-api-key\n  description: Api keys provide higher access to rate limits. To obtain an api key, sign up\n    for an account at https://avacloud.io/.\n  sources:\n  - openapi/ava-labs-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/authentication/ava-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Blockchain
- Avalanche
- Web3
- Data API
- Developer Platform
- Infrastructure
---
