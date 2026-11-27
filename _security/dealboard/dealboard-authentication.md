---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dealboard-deals-api-openapi.yml
  format: yaml
  label: Dealboard Deals API
  slug: dealboard-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-deals-api-openapi.yml
- filename: dealboard-reports-api-openapi.yml
  format: yaml
  label: Dealboard Reports API
  slug: dealboard-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-reports-api-openapi.yml
- filename: dealboard-templates-api-openapi.yml
  format: yaml
  label: Dealboard Templates API
  slug: dealboard-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-templates-api-openapi.yml
- filename: dealboard-auth-api-openapi.yml
  format: yaml
  label: Dealboard Auth API
  slug: dealboard-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-auth-api-openapi.yml
- filename: dealboard-boards-api-openapi.yml
  format: yaml
  label: Dealboard Boards API
  slug: dealboard-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-boards-api-openapi.yml
- filename: dealboard-dealboard-api-api-openapi.yml
  format: yaml
  label: Dealboard Dealboard API
  slug: dealboard-dealboard-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-dealboard-api-api-openapi.yml
- filename: dealboard-leads-api-openapi.yml
  format: yaml
  label: Dealboard Leads API
  slug: dealboard-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-leads-api-openapi.yml
- filename: dealboard-match-api-openapi.yml
  format: yaml
  label: Dealboard Match API
  slug: dealboard-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-match-api-openapi.yml
- filename: dealboard-notes-api-openapi.yml
  format: yaml
  label: Dealboard Notes API
  slug: dealboard-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-notes-api-openapi.yml
- filename: dealboard-webhooks-api-openapi.yml
  format: yaml
  label: Dealboard Webhooks API
  slug: dealboard-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dealboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dealboard secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dealboard
provider_slug: dealboard
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/dealboard-boards-api-openapi.yml
  - openapi/dealboard-dealboard-api-api-openapi.yml
  - openapi/dealboard-deals-api-openapi.yml
  - openapi/dealboard-openapi.json
  - openapi/dealboard-reports-api-openapi.yml
  - openapi/dealboard-templates-api-openapi.yml
  type: http
slug: dealboard-authentication
source_filename: dealboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/dealboard-boards-api-openapi.yml, openapi/dealboard-dealboard-api-api-openapi.yml,\n  openapi/dealboard-deals-api-openapi.yml, openapi/dealboard-openapi.json, openapi/dealboard-reports-api-openapi.yml,\n  openapi/dealboard-templates-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dealboard-boards-api-openapi.yml\n  - openapi/dealboard-dealboard-api-api-openapi.yml\n  - openapi/dealboard-deals-api-openapi.yml\n  - openapi/dealboard-openapi.json\n  - openapi/dealboard-reports-api-openapi.yml\n  - openapi/dealboard-templates-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dealboard/authentication/dealboard-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- CRM
- Sales
- Artificial Intelligence
- Integration
---
