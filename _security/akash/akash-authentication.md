---
api_key_in:
- header
api_specs:
- filename: akash-console-deployment-api.json
  format: json
  label: Akash Console Deployment API
  slug: akash-console-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-console-deployment-api.json
- filename: akash-blockchain-rest-api.yaml
  format: yaml
  label: Akash Blockchain REST API
  slug: akash-blockchain-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-blockchain-rest-api.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Akash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akash Network secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Akash Network
provider_slug: akash
scheme_count: 5
schemes:
- name: kms
  scheme: basic
  sources:
  - openapi/akash-blockchain-rest-api.yaml
  type: http
- bearerFormat: JWT
  description: 'JWT token for authenticated users, sent in "Authorization: Bearer %token" header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/akash-console-deployment-api.json
  type: http
- description: API key for programmatic access.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/akash-console-deployment-api.json
  type: apiKey
- in: header
  name: x-user-id
  parameter: x-user-id
  sources:
  - openapi/akash-console-deployment-api.json
  - openapi/akash-notifications-api.json
  type: apiKey
- in: header
  name: x-owner-address
  parameter: x-owner-address
  sources:
  - openapi/akash-console-deployment-api.json
  - openapi/akash-notifications-api.json
  type: apiKey
slug: akash-authentication
source_filename: akash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akash-blockchain-rest-api.yaml, openapi/akash-console-deployment-api.json, openapi/akash-notifications-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: kms\n  type: http\n  scheme: basic\n  sources:\n  - openapi/akash-blockchain-rest-api.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT token for authenticated users, sent in \"Authorization: Bearer %token\" header.'\n  sources:\n  - openapi/akash-console-deployment-api.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for programmatic access.\n  sources:\n  - openapi/akash-console-deployment-api.json\n- name: x-user-id\n  type: apiKey\n  in: header\n  parameter: x-user-id\n  sources:\n  - openapi/akash-console-deployment-api.json\n  - openapi/akash-notifications-api.json\n- name: x-owner-address\n  type: apiKey\n  in: header\n\
  \  parameter: x-owner-address\n  sources:\n  - openapi/akash-console-deployment-api.json\n  - openapi/akash-notifications-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/authentication/akash-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Cloud Computing
- Decentralized
- Blockchain
- Kubernetes
- GPU
- AI Inference
- Cosmos
- Web3
---
