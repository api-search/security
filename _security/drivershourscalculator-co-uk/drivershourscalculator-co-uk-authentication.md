---
anonymous_access: false
api_key_in: []
api_specs:
- filename: drivershourscalculator-co-uk-calculator-api-openapi.yml
  format: yaml
  label: Drivers' Hours Calculator Calculator API
  slug: drivershourscalculator-co-uk-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivershourscalculator-co-uk/openapi/drivershourscalculator-co-uk-calculator-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Drivershourscalculator Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drivers' Hours Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drivers' Hours Calculator
provider_slug: drivershourscalculator-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/drivershourscalculator-co-uk-openapi.json
  type: http
slug: drivershourscalculator-co-uk-authentication
source_filename: drivershourscalculator-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/drivershourscalculator-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/drivershourscalculator-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drivershourscalculator-co-uk/authentication/drivershourscalculator-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Drivers
- EU
- HGV
- Compliance
- Calculator
---
