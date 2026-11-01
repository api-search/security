---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fabtally-com-attest-api-openapi.yml
  format: yaml
  label: fabtally-com Attest API
  slug: fabtally-com-attest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-attest-api-openapi.yml
- filename: fabtally-com-dfm-api-openapi.yml
  format: yaml
  label: fabtally-com DFM API
  slug: fabtally-com-dfm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-dfm-api-openapi.yml
- filename: fabtally-com-discovery-api-openapi.yml
  format: yaml
  label: fabtally-com Discovery API
  slug: fabtally-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-discovery-api-openapi.yml
- filename: fabtally-com-quote-api-openapi.yml
  format: yaml
  label: fabtally-com Quote API
  slug: fabtally-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-quote-api-openapi.yml
- filename: fabtally-com-slice-api-openapi.yml
  format: yaml
  label: fabtally-com Slice API
  slug: fabtally-com-slice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-slice-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fabtally Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: fabtally-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: fabtally-com
provider_slug: fabtally-com
scheme_count: 1
schemes:
- description: Payment authentication via x402 protocol; agents pay per call in USDC on Base. Unpaid requests receive HTTP 402 with price and payment details.
  name: x402
  type: custom
slug: fabtally-com-authentication
source_filename: fabtally-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://fabtally.com/\nschemes:\n  - type: custom\n    name: x402\n    description: \"Payment authentication via x402 protocol; agents pay per call in USDC on Base. Unpaid requests receive HTTP 402 with price and payment details.\"\n"
source_yaml_url: https://artifacts.apis.io/fabtally-com/authentication/fabtally-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- 3D-printing
- Slicing
- Quotes
- API
- Manufacturing
---
