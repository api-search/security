---
api_key_in:
- header
- query
api_specs:
- filename: enso-ccip-api-openapi.yml
  format: yaml
  label: Enso ccip API
  slug: enso-ccip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-ccip-api-openapi.yml
- filename: enso-cctp-api-openapi.yml
  format: yaml
  label: Enso cctp API
  slug: enso-cctp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-cctp-api-openapi.yml
- filename: enso-layerzero-api-openapi.yml
  format: yaml
  label: Enso layerzero API
  slug: enso-layerzero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-layerzero-api-openapi.yml
- filename: enso-metadata-api-openapi.yml
  format: yaml
  label: Enso metadata API
  slug: enso-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-metadata-api-openapi.yml
- filename: enso-projects-api-openapi.yml
  format: yaml
  label: Enso projects API
  slug: enso-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-projects-api-openapi.yml
- filename: enso-relay-api-openapi.yml
  format: yaml
  label: Enso relay API
  slug: enso-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-relay-api-openapi.yml
- filename: enso-shortcuts-api-openapi.yml
  format: yaml
  label: Enso shortcuts API
  slug: enso-shortcuts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-shortcuts-api-openapi.yml
- filename: enso-standards-api-openapi.yml
  format: yaml
  label: Enso standards API
  slug: enso-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-standards-api-openapi.yml
- filename: enso-wallet-api-openapi.yml
  format: yaml
  label: Enso wallet API
  slug: enso-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enso secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enso
provider_slug: enso
scheme_count: 1
schemes:
- alt_location: query parameter apikey=<API_KEY>
  bearerFormat: apiKey
  location: Authorization header, "Bearer <API_KEY>"
  name: bearer
  scheme: bearer
  sources:
  - openapi/enso-openapi-original.json
  type: http
slug: enso-authentication
source_filename: enso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/enso-openapi-original.json\ndocs: https://docs.enso.build/pages/build/get-started/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  - query\n  scheme: bearer\n  get_key: https://developers.enso.build/\n  rate_limit: 10 rps (600 requests/minute), increasable on request; 429 on exceed\n  demo_key: 1e02632d-6feb-4a75-a157-documentation (1 rps, documentation only)\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  location: Authorization header, \"Bearer <API_KEY>\"\n  alt_location: query parameter apikey=<API_KEY>\n  sources:\n  - openapi/enso-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/authentication/enso-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto Web3
- DeFi
- Blockchain
- Cross-Chain
- Smart Contracts
- Transaction Routing
- Web3 Infrastructure
- Onchain
---
