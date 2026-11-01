---
anonymous_access: false
api_key_in: []
api_specs:
- filename: toolaby-app-analytics-api-openapi.yml
  format: yaml
  label: toolaby-app Analytics API
  slug: toolaby-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-analytics-api-openapi.yml
- filename: toolaby-app-customers-api-openapi.yml
  format: yaml
  label: toolaby-app Customers API
  slug: toolaby-app-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-customers-api-openapi.yml
- filename: toolaby-app-grants-api-openapi.yml
  format: yaml
  label: toolaby-app Grants API
  slug: toolaby-app-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-grants-api-openapi.yml
- filename: toolaby-app-uses-api-openapi.yml
  format: yaml
  label: toolaby-app Uses API
  slug: toolaby-app-uses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-uses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Toolaby App Authentication
name_suffix: Authentication
oauth_flows: []
overview: toolaby-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: toolaby-app
provider_slug: toolaby-app
scheme_count: 1
schemes:
- description: 'An API key from the dashboard: wk_test_… or wk_live_….'
  name: bearer
  scheme: bearer
  sources:
  - openapi/toolaby-app-openapi.json
  type: http
slug: toolaby-app-authentication
source_filename: toolaby-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/toolaby-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'An API key from the dashboard: wk_test_… or wk_live_….'\n  sources:\n  - openapi/toolaby-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/toolaby-app/authentication/toolaby-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Chrome-Extension
- Stripe
- Licensing
---
