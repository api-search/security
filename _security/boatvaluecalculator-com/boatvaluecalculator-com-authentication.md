---
anonymous_access: false
api_key_in: []
api_specs:
- filename: boatvaluecalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Boat Value Calculator Calculator API
  slug: boatvaluecalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boatvaluecalculator-com/openapi/boatvaluecalculator-com-calculator-api-openapi.yml
- filename: boatvaluecalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Boat Value Calculator Enquiry API
  slug: boatvaluecalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boatvaluecalculator-com/openapi/boatvaluecalculator-com-enquiry-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Boatvaluecalculator Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boat Value Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boat Value Calculator
provider_slug: boatvaluecalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/boatvaluecalculator-com-openapi.json
  type: http
slug: boatvaluecalculator-com-authentication
source_filename: boatvaluecalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/boatvaluecalculator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/boatvaluecalculator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/boatvaluecalculator-com/authentication/boatvaluecalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Boat
- Valuation
- Finance
- Marine
- Calculator
---
