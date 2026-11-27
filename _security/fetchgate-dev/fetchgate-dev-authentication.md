---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fetchgate-dev-buy-api-openapi.yml
  format: yaml
  label: Fetchgate Buy API
  slug: fetchgate-dev-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-buy-api-openapi.yml
- filename: fetchgate-dev-download-api-openapi.yml
  format: yaml
  label: Fetchgate Download API
  slug: fetchgate-dev-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-download-api-openapi.yml
- filename: fetchgate-dev-llms-txt-api-openapi.yml
  format: yaml
  label: Fetchgate Llms.txt API
  slug: fetchgate-dev-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-llms-txt-api-openapi.yml
- filename: fetchgate-dev-mcp-api-openapi.yml
  format: yaml
  label: Fetchgate MCP API
  slug: fetchgate-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-mcp-api-openapi.yml
- filename: fetchgate-dev-meta-api-openapi.yml
  format: yaml
  label: Fetchgate Meta API
  slug: fetchgate-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-meta-api-openapi.yml
- filename: fetchgate-dev-openapi-json-api-openapi.yml
  format: yaml
  label: Fetchgate Openapi.json API
  slug: fetchgate-dev-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-openapi-json-api-openapi.yml
- filename: fetchgate-dev-products-api-openapi.yml
  format: yaml
  label: Fetchgate Products API
  slug: fetchgate-dev-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-products-api-openapi.yml
- filename: fetchgate-dev-read-api-openapi.yml
  format: yaml
  label: Fetchgate Read API
  slug: fetchgate-dev-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-read-api-openapi.yml
- filename: fetchgate-dev-scan-api-openapi.yml
  format: yaml
  label: Fetchgate Scan API
  slug: fetchgate-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-scan-api-openapi.yml
- filename: fetchgate-dev-token-api-openapi.yml
  format: yaml
  label: Fetchgate Token API
  slug: fetchgate-dev-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-token-api-openapi.yml
- filename: fetchgate-dev-x402-api-openapi.yml
  format: yaml
  label: Fetchgate X402 API
  slug: fetchgate-dev-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchgate-dev/openapi/fetchgate-dev-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fetchgate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fetchgate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fetchgate
provider_slug: fetchgate-dev
scheme_count: 1
schemes:
- description: 'Optional API key for authenticated/paid access. TODO: pay-per-request via x402 is planned as an alternative to a pre-provisioned key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fetchgate-dev-openapi.json
  type: http
slug: fetchgate-dev-authentication
source_filename: fetchgate-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fetchgate-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Optional API key for authenticated/paid access. TODO: pay-per-request via x402\n    is planned as an alternative to a pre-provisioned key.'\n  sources:\n  - openapi/fetchgate-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fetchgate-dev/authentication/fetchgate-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Goods
- Payments
- AI Agents
- Marketplace
---
