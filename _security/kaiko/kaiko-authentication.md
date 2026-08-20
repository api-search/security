---
api_key_in:
- header
api_specs:
- filename: kaiko-canton-oracle-api-openapi.yml
  format: yaml
  label: Kaiko Canton Oracle API
  slug: kaiko-canton-oracle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/openapi/kaiko-canton-oracle-api-openapi.yml
- filename: kaiko-index-reference-data-api-openapi.yml
  format: yaml
  label: Kaiko Index Reference Data API
  slug: kaiko-index-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/openapi/kaiko-index-reference-data-api-openapi.yml
- filename: kaiko-indices-api-openapi.yml
  format: yaml
  label: Kaiko Indices API
  slug: kaiko-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/openapi/kaiko-indices-api-openapi.yml
- filename: kaiko-supply-api-openapi.yml
  format: yaml
  label: Kaiko Supply API
  slug: kaiko-supply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/openapi/kaiko-supply-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kaiko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaiko secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kaiko
provider_slug: kaiko
scheme_count: 1
schemes:
- description: Kaiko client API key delivered in the X-Api-Key header.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/kaiko-canton-oracle-api-openapi.yml
  - openapi/kaiko-index-reference-data-api-openapi.yml
  - openapi/kaiko-indices-api-openapi.yml
  - openapi/kaiko-supply-api-openapi.yml
  type: apiKey
slug: kaiko-authentication
source_filename: kaiko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/ security schemes\ndocs: https://docs.kaiko.com/rest-api/general/getting-started/authentication.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  All Kaiko REST requests carry the client API key in the X-Api-Key header; each Market\n  Data endpoint lives under its own hostname. Keys are provisioned via Kaiko's sales-led\n  onboarding (no self-serve signup, no OAuth). Kaiko Stream (gRPC) authenticates with the\n  same API key supplied via the per-language SDKs\n  (https://docs.kaiko.com/stream/general/general-information/api-key.md).\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Kaiko client API key delivered in the X-Api-Key header.\n  sources:\n  - openapi/kaiko-canton-oracle-api-openapi.yml\n  - openapi/kaiko-index-reference-data-api-openapi.yml\n  - openapi/kaiko-indices-api-openapi.yml\n  - openapi/kaiko-supply-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/authentication/kaiko-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- Market Data
- Institutional
- FX
- Indices
- Onchain
- Streaming
---
