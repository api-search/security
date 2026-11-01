---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: gender-api-country-of-origin-api-openapi.yml
  format: yaml
  label: Gender API Country Of Origin API
  slug: gender-api-country-of-origin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-country-of-origin-api-openapi.yml
- filename: gender-api-gender-api-openapi.yml
  format: yaml
  label: Gender API Gender API
  slug: gender-api-gender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-gender-api-openapi.yml
- filename: gender-api-statistic-api-openapi.yml
  format: yaml
  label: Gender API Statistic API
  slug: gender-api-statistic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-statistic-api-openapi.yml
- filename: gender-api-signup-api-openapi.yml
  format: yaml
  label: Gender API Signup API
  slug: gender-api-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-signup-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gender Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gender API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gender API
provider_slug: gender-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/gender-api-openapi.yml
  type: apiKey
slug: gender-api-authentication
source_filename: gender-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gender-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/gender-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gender-api/authentication/gender-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Demographics
- Gender
- Identity
- Name
- Personal Data
---
