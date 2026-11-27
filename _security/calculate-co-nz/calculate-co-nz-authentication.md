---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: calculate-co-nz-calculators-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Calculators API
  slug: calculate-co-nz-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-calculators-api-openapi.yml
- filename: calculate-co-nz-discovery-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Discovery API
  slug: calculate-co-nz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-discovery-api-openapi.yml
- filename: calculate-co-nz-reference-data-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Reference data API
  slug: calculate-co-nz-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-reference-data-api-openapi.yml
- filename: calculate-co-nz-service-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Service API
  slug: calculate-co-nz-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-service-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Calculate.co.nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calculate.co.nz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calculate.co.nz
provider_slug: calculate-co-nz
scheme_count: 1
schemes:
- description: Optional. Identifies your calls and raises your hourly limit from 120 to 5000 requests. Request one from contact@calculate.co.nz
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/calculate-co-nz-openapi.json
  type: apiKey
slug: calculate-co-nz-authentication
source_filename: calculate-co-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/calculate-co-nz-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional. Identifies your calls and raises your hourly limit from 120 to 5000\n    requests. Request one from contact@calculate.co.nz\n  sources:\n  - openapi/calculate-co-nz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/calculate-co-nz/authentication/calculate-co-nz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Finance
- Calculators
- New Zealand
- Free
- Education
---
