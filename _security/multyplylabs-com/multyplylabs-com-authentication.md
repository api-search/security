---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: multyplylabs-com-aggregate-api-openapi.yml
  format: yaml
  label: Multyply Labs Aggregate API
  slug: multyplylabs-com-aggregate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-aggregate-api-openapi.yml
- filename: multyplylabs-com-catalog-api-openapi.yml
  format: yaml
  label: Multyply Labs Catalog API
  slug: multyplylabs-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-catalog-api-openapi.yml
- filename: multyplylabs-com-company-api-openapi.yml
  format: yaml
  label: Multyply Labs Company API
  slug: multyplylabs-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-company-api-openapi.yml
- filename: multyplylabs-com-compare-api-openapi.yml
  format: yaml
  label: Multyply Labs Compare API
  slug: multyplylabs-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-compare-api-openapi.yml
- filename: multyplylabs-com-health-api-openapi.yml
  format: yaml
  label: Multyply Labs Health API
  slug: multyplylabs-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-health-api-openapi.yml
- filename: multyplylabs-com-insight-api-openapi.yml
  format: yaml
  label: Multyply Labs Insight API
  slug: multyplylabs-com-insight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-insight-api-openapi.yml
- filename: multyplylabs-com-insights-api-openapi.yml
  format: yaml
  label: Multyply Labs Insights API
  slug: multyplylabs-com-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-insights-api-openapi.yml
- filename: multyplylabs-com-screen-api-openapi.yml
  format: yaml
  label: Multyply Labs Screen API
  slug: multyplylabs-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-screen-api-openapi.yml
- filename: multyplylabs-com-spotlight-api-openapi.yml
  format: yaml
  label: Multyply Labs Spotlight API
  slug: multyplylabs-com-spotlight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multyplylabs-com/openapi/multyplylabs-com-spotlight-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Multyply Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Multyply Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Multyply Labs
provider_slug: multyplylabs-com
scheme_count: 1
schemes:
- description: API key (help@multyplylabs.com). A request carrying a valid key is served without payment; without one, a paid route answers 402 with an x402 payment challenge.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/multyplylabs-com-openapi.json
  type: apiKey
slug: multyplylabs-com-authentication
source_filename: multyplylabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/multyplylabs-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key (help@multyplylabs.com). A request carrying a valid key is served without\n    payment; without one, a paid route answers 402 with an x402 payment challenge.\n  sources:\n  - openapi/multyplylabs-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/multyplylabs-com/authentication/multyplylabs-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- College Counseling
- SEC Data
- Public Data
- Agents
- Financial Data
---
