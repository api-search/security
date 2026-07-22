---
api_key_in:
- header
api_specs:
- filename: terminal-3-openapi.yml
  format: yaml
  label: Terminal 3 API
  slug: terminal-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-3/refs/heads/main/openapi/terminal-3-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Terminal 3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal 3 secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Terminal 3
provider_slug: terminal-3
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Default authentication for the T3 REST API (Authorization: Bearer <token>).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/terminal-3-openapi.yml
  type: http
- description: Required on specific endpoints such as user creation. Obtain via enterprise@terminal3.io.
  in: header
  name: apiKeyAuth
  parameter_name: x-api-token
  sources:
  - openapi/terminal-3-openapi.yml
  type: apiKey
slug: terminal-3-authentication
source_filename: terminal-3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.terminal3.io/developers/adk/reference\ndocs: https://docs.terminal3.io/api-reference/t3-api/getting-started\nnote: >-\n  Terminal 3 REST API authenticates with a bearer JWT by default; specific\n  endpoints (e.g. user creation) additionally require an x-api-token header.\n  Request an API key from enterprise@terminal3.io or the self-serve claim page.\n  The ADK SDK layer authenticates separately via SIWE (Sign-In With Ethereum,\n  EIP-4361) to obtain a tenant DID.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  http_schemes: [bearer]\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Default authentication for the T3 REST API (Authorization: Bearer <token>).\"\n    sources: [openapi/terminal-3-openapi.yml]\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-token\n    description: Required on specific endpoints\
  \ such as user creation. Obtain via enterprise@terminal3.io.\n    sources: [openapi/terminal-3-openapi.yml]\nsdk_auth:\n  - method: SIWE\n    standard: EIP-4361 (Sign-In With Ethereum)\n    description: >-\n      The @terminal3/t3n-sdk handshake/authenticate flow signs a login challenge\n      (metamask_sign) to derive an authenticated tenant DID (did:t3n:...).\n    source: https://docs.terminal3.io/developers/adk/get-started/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-3/refs/heads/main/authentication/terminal-3-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Identity
- Decentralized Identity
- Verifiable Credentials
- OpenID Connect
- KYC
- AML
- Confidential Computing
- AI Agents
- Privacy
- Web3
- DID
---
