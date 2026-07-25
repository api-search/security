---
api_key_in: []
api_specs:
- filename: ava-protocol-auth-api-openapi.yml
  format: yaml
  label: Ava Protocol Auth API
  slug: ava-protocol-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-auth-api-openapi.yml
- filename: ava-protocol-executions-api-openapi.yml
  format: yaml
  label: Ava Protocol Executions API
  slug: ava-protocol-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-executions-api-openapi.yml
- filename: ava-protocol-health-api-openapi.yml
  format: yaml
  label: Ava Protocol Health API
  slug: ava-protocol-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-health-api-openapi.yml
- filename: ava-protocol-nodes-api-openapi.yml
  format: yaml
  label: Ava Protocol Nodes API
  slug: ava-protocol-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-nodes-api-openapi.yml
- filename: ava-protocol-operators-api-openapi.yml
  format: yaml
  label: Ava Protocol Operators API
  slug: ava-protocol-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-operators-api-openapi.yml
- filename: ava-protocol-secrets-api-openapi.yml
  format: yaml
  label: Ava Protocol Secrets API
  slug: ava-protocol-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-secrets-api-openapi.yml
- filename: ava-protocol-tokens-api-openapi.yml
  format: yaml
  label: Ava Protocol Tokens API
  slug: ava-protocol-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-tokens-api-openapi.yml
- filename: ava-protocol-triggers-api-openapi.yml
  format: yaml
  label: Ava Protocol Triggers API
  slug: ava-protocol-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-triggers-api-openapi.yml
- filename: ava-protocol-wallets-api-openapi.yml
  format: yaml
  label: Ava Protocol Wallets API
  slug: ava-protocol-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-wallets-api-openapi.yml
- filename: ava-protocol-workflows-api-openapi.yml
  format: yaml
  label: Ava Protocol Workflows API
  slug: ava-protocol-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-workflows-api-openapi.yml
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
