---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hirehouse-xyz-openapi.json
  format: json
  label: HireHouse Public Jobs API
  slug: hirehouse-public-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hirehouse-xyz/openapi/hirehouse-xyz-openapi.json
- filename: hirehouse-xyz-jobs-api-openapi.yml
  format: yaml
  label: HireHouse Jobs API
  slug: hirehouse-xyz-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hirehouse-xyz/openapi/hirehouse-xyz-jobs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: HireHouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: HireHouse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HireHouse
provider_slug: hirehouse-xyz
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-HireHouse-Key
  sources:
  - openapi/hirehouse-xyz-openapi.json
  type: apiKey
slug: hirehouse-xyz-authentication
source_filename: hirehouse-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/hirehouse-xyz-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-HireHouse-Key\n  sources:\n  - openapi/hirehouse-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hirehouse-xyz/authentication/hirehouse-xyz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Job Board
- Hiring
- AI Interview
- Fast Track
- United Arab Emirates
- India
---
