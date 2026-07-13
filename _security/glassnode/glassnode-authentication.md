---
api_key_in:
- header
api_specs:
- filename: glassnode-openapi.yml
  format: yaml
  label: Glassnode Metrics API
  slug: metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Glassnode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glassnode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glassnode
provider_slug: glassnode
scheme_count: 1
schemes:
- description: Glassnode API key with institutional or paid plan.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/glassnode-openapi.yml
  type: apiKey
slug: glassnode-authentication
source_filename: glassnode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glassnode-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Glassnode API key with institutional or paid plan.\n  sources:\n  - openapi/glassnode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/authentication/glassnode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- On-Chain
- Analytics
- Metrics
- Bitcoin
- Ethereum
- Institutional
---
