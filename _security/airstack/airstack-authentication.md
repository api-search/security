---
api_key_in:
- header
api_specs:
- filename: farcaster-hub-rest-api.json
  format: json
  label: Airstack Farcaster Hub API
  slug: airstack-farcaster-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-hub-rest-api.json
- filename: farcaster-webhooks-api.json
  format: json
  label: Airstack Farcaster Webhooks API
  slug: airstack-farcaster-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-webhooks-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airstack secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Airstack
provider_slug: airstack
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-airstack-hubs
  sources:
  - openapi/farcaster-hub-rest-api.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/farcaster-webhooks-api.json
  type: apiKey
slug: airstack-authentication
source_filename: airstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/farcaster-hub-rest-api.json, openapi/farcaster-webhooks-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-airstack-hubs\n  sources:\n  - openapi/farcaster-hub-rest-api.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/farcaster-webhooks-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/authentication/airstack-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Web3
- Blockchain
- GraphQL
- NFT
- Tokens
- On-Chain Data
- Ethereum
- Polygon
- Base
- ENS
- POAP
- Social Graph
- Wallet
- Identity
---
