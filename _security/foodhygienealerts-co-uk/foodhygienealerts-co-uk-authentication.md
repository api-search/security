---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foodhygienealerts-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Food Hygiene Alerts Enquiry API
  slug: foodhygienealerts-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodhygienealerts-co-uk/openapi/foodhygienealerts-co-uk-enquiry-api-openapi.yml
- filename: foodhygienealerts-co-uk-guide-api-openapi.yml
  format: yaml
  label: Food Hygiene Alerts Guide API
  slug: foodhygienealerts-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodhygienealerts-co-uk/openapi/foodhygienealerts-co-uk-guide-api-openapi.yml
- filename: foodhygienealerts-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Food Hygiene Alerts MCP API
  slug: foodhygienealerts-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodhygienealerts-co-uk/openapi/foodhygienealerts-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Food Hygiene Alerts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Food Hygiene Alerts secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Food Hygiene Alerts
provider_slug: foodhygienealerts-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/foodhygienealerts-co-uk-openapi.json
  type: http
slug: foodhygienealerts-co-uk-authentication
source_filename: foodhygienealerts-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/foodhygienealerts-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/foodhygienealerts-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/foodhygienealerts-co-uk/authentication/foodhygienealerts-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Food Hygiene
- United Kingdom
- Public Data
- Health
- Compliance
---
