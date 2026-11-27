---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: No Vig Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: No Vig Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: No Vig Calculator
provider_slug: fairoddscalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/fairoddscalculator-com-openapi.json
  type: http
slug: fairoddscalculator-com-authentication
source_filename: fairoddscalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fairoddscalculator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/fairoddscalculator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fairoddscalculator-com/authentication/fairoddscalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Betting
- Calculator
- Sports
- Odds
- Finance
---
