---
api_key_in:
- header
api_specs:
- filename: akash-network-bids-api-openapi.yml
  format: yaml
  label: Akash Network Bids API
  slug: akash-network-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/openapi/akash-network-bids-api-openapi.yml
- filename: akash-network-deployments-api-openapi.yml
  format: yaml
  label: Akash Network Deployments API
  slug: akash-network-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/openapi/akash-network-deployments-api-openapi.yml
- filename: akash-network-leases-api-openapi.yml
  format: yaml
  label: Akash Network Leases API
  slug: akash-network-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/openapi/akash-network-leases-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Akash Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akash Network secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Akash Network
provider_slug: akash-network
scheme_count: 1
schemes:
- description: Akash Console API key passed on every request.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/akash-network-openapi.yml
  type: apiKey
slug: akash-network-authentication
source_filename: akash-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akash-network-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Akash Console API key passed on every request.\n  sources:\n  - openapi/akash-network-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/authentication/akash-network-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Decentralized Cloud
- GPU
- Compute
- DePIN
- Cosmos
- Crypto
- Marketplace
---
