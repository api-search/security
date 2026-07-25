---
api_key_in:
- header
api_specs:
- filename: airstack-casts-api-openapi.yml
  format: yaml
  label: Airstack Casts API
  slug: airstack-casts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-casts-api-openapi.yml
- filename: airstack-fids-api-openapi.yml
  format: yaml
  label: Airstack FIDs API
  slug: airstack-fids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-fids-api-openapi.yml
- filename: airstack-hubevents-api-openapi.yml
  format: yaml
  label: Airstack HubEvents API
  slug: airstack-hubevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-hubevents-api-openapi.yml
- filename: airstack-links-api-openapi.yml
  format: yaml
  label: Airstack Links API
  slug: airstack-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-links-api-openapi.yml
- filename: airstack-onchainevents-api-openapi.yml
  format: yaml
  label: Airstack OnChainEvents API
  slug: airstack-onchainevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-onchainevents-api-openapi.yml
- filename: airstack-reactions-api-openapi.yml
  format: yaml
  label: Airstack Reactions API
  slug: airstack-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-reactions-api-openapi.yml
- filename: airstack-storage-api-openapi.yml
  format: yaml
  label: Airstack Storage API
  slug: airstack-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-storage-api-openapi.yml
- filename: airstack-submitmessage-api-openapi.yml
  format: yaml
  label: Airstack SubmitMessage API
  slug: airstack-submitmessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-submitmessage-api-openapi.yml
- filename: airstack-userdata-api-openapi.yml
  format: yaml
  label: Airstack UserData API
  slug: airstack-userdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-userdata-api-openapi.yml
- filename: airstack-usernames-api-openapi.yml
  format: yaml
  label: Airstack Usernames API
  slug: airstack-usernames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-usernames-api-openapi.yml
- filename: airstack-validatemessage-api-openapi.yml
  format: yaml
  label: Airstack ValidateMessage API
  slug: airstack-validatemessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-validatemessage-api-openapi.yml
- filename: airstack-verifications-api-openapi.yml
  format: yaml
  label: Airstack Verifications API
  slug: airstack-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-verifications-api-openapi.yml
- filename: airstack-webhooks-api-openapi.yml
  format: yaml
  label: Airstack Webhooks API
  slug: airstack-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/airstack-webhooks-api-openapi.yml
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
