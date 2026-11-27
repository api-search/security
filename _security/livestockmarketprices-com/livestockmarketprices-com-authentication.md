---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: livestockmarketprices-com-benchmarks-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Benchmarks API
  slug: livestockmarketprices-com-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-benchmarks-api-openapi.yml
- filename: livestockmarketprices-com-coverage-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Coverage API
  slug: livestockmarketprices-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-coverage-api-openapi.yml
- filename: livestockmarketprices-com-data-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Data API
  slug: livestockmarketprices-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-data-api-openapi.yml
- filename: livestockmarketprices-com-healthz-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Healthz API
  slug: livestockmarketprices-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-healthz-api-openapi.yml
- filename: livestockmarketprices-com-methodologies-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Methodologies API
  slug: livestockmarketprices-com-methodologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-methodologies-api-openapi.yml
- filename: livestockmarketprices-com-openapi-json-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Openapi.json API
  slug: livestockmarketprices-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-openapi-json-api-openapi.yml
- filename: livestockmarketprices-com-prices-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Prices API
  slug: livestockmarketprices-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-prices-api-openapi.yml
- filename: livestockmarketprices-com-reports-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Reports API
  slug: livestockmarketprices-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-reports-api-openapi.yml
- filename: livestockmarketprices-com-valuations-api-openapi.yml
  format: yaml
  label: Livestock Market Prices Valuations API
  slug: livestockmarketprices-com-valuations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livestockmarketprices-com/openapi/livestockmarketprices-com-valuations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Livestock Market Prices Authentication
name_suffix: Authentication
oauth_flows: []
overview: Livestock Market Prices secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Livestock Market Prices
provider_slug: livestockmarketprices-com
scheme_count: 1
schemes:
- description: A signed-in LMP Member or Pro session.
  in: cookie
  name: memberSession
  parameter: lmp_session
  sources:
  - openapi/livestockmarketprices-com-openapi.json
  type: apiKey
slug: livestockmarketprices-com-authentication
source_filename: livestockmarketprices-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/livestockmarketprices-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: memberSession\n  type: apiKey\n  in: cookie\n  parameter: lmp_session\n  description: A signed-in LMP Member or Pro session.\n  sources:\n  - openapi/livestockmarketprices-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/livestockmarketprices-com/authentication/livestockmarketprices-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Livestock
- Agriculture
- Market Data
- Prices
---
