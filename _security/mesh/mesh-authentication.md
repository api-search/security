---
api_key_in:
- header
api_specs:
- filename: mesh-assets-api-openapi.yml
  format: yaml
  label: Mesh Assets API
  slug: mesh-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-assets-api-openapi.yml
- filename: mesh-balance-api-openapi.yml
  format: yaml
  label: Mesh Balance API
  slug: mesh-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-balance-api-openapi.yml
- filename: mesh-brokeraccountdetail-api-openapi.yml
  format: yaml
  label: Mesh BrokerAccountDetail API
  slug: mesh-brokeraccountdetail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-brokeraccountdetail-api-openapi.yml
- filename: mesh-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Managed Account Authentication API
  slug: mesh-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-managed-account-authentication-api-openapi.yml
- filename: mesh-managed-transfers-api-openapi.yml
  format: yaml
  label: Mesh Managed Transfers API
  slug: mesh-managed-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-managed-transfers-api-openapi.yml
- filename: mesh-portfolio-api-openapi.yml
  format: yaml
  label: Mesh Portfolio API
  slug: mesh-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-portfolio-api-openapi.yml
- filename: mesh-self-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Self Managed Account Authentication API
  slug: mesh-self-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-self-managed-account-authentication-api-openapi.yml
- filename: mesh-transactions-api-openapi.yml
  format: yaml
  label: Mesh Transactions API
  slug: mesh-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-transactions-api-openapi.yml
- filename: mesh-transfers-api-openapi.yml
  format: yaml
  label: Mesh Transfers API
  slug: mesh-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-transfers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mesh secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mesh
provider_slug: mesh
scheme_count: 2
schemes:
- description: Contact Mesh to get client Secret
  in: header
  name: Client-Secret
  parameter: X-Client-Secret
  sources:
  - openapi/mesh-integration-api-openapi.json
  type: apiKey
- description: Contact Mesh to get client Id
  in: header
  name: Client-Id
  parameter: X-Client-Id
  sources:
  - openapi/mesh-integration-api-openapi.json
  type: apiKey
slug: mesh-authentication
source_filename: mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mesh-integration-api-openapi.json\ndocs: https://docs.meshconnect.com/build/prepare-to-build\nnotes: >-\n  Server-to-server calls to the Mesh Connect Integration API authenticate with two\n  API-key headers issued in the Mesh dashboard (Account > API keys): X-Client-Id and\n  X-Client-Secret. Sandbox and production keys are separate. Registered-client (sub-client)\n  calls additionally use a short-lived auth token obtained via POST\n  /api/v1/auth-token (see api-reference/auth-token/generate-auth-token). Link Tokens\n  (POST /api/v1/linktoken) are short-lived (10 min) single-use tokens minted server-side\n  and handed to the client SDK to launch Link. No OAuth2 is exposed on Mesh's own API\n  (OAuth is used internally by Mesh when connecting end users to underlying integrations).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Client-Secret\n  type: apiKey\n  in: header\n  parameter: X-Client-Secret\n\
  \  description: Contact Mesh to get client Secret\n  sources:\n  - openapi/mesh-integration-api-openapi.json\n- name: Client-Id\n  type: apiKey\n  in: header\n  parameter: X-Client-Id\n  description: Contact Mesh to get client Id\n  sources:\n  - openapi/mesh-integration-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/authentication/mesh-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Crypto
- Cryptocurrency
- Payments
- Digital Assets
- Financial Services
- Wallets
- Exchanges
- Transfers
- Stablecoins
- Embedded Finance
- Fintech
- On-Ramp
- Blockchain
---
