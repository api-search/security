---
api_key_in: []
api_specs:
- filename: ava-protocol-avs-openapi-original.yml
  format: yaml
  label: Ava Protocol AVS API
  slug: ava-protocol-avs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-avs-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ava Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ava Protocol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ava Protocol
provider_slug: ava-protocol
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT bearer token. Obtained via `POST /auth:exchange` (wallet

    signature flow) or via the operator-run `create-api-key` CLI

    (long-lived, server-to-server). Send on every request as

    `Authorization: Bearer <jwt>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ava-protocol-avs-openapi-original.yml
  type: http
slug: ava-protocol-authentication
source_filename: ava-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/ava-protocol-avs-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT bearer token. Obtained via `POST /auth:exchange` (wallet\n    signature flow) or via the operator-run `create-api-key` CLI\n    (long-lived, server-to-server). Send on every request as\n    `Authorization: Bearer <jwt>`.\n  sources:\n  - openapi/ava-protocol-avs-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/authentication/ava-protocol-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Blockchain
- DeFi
- Automation
- Web3
- Ethereum
- Smart Wallets
- Workflows
- AI Agents
---
