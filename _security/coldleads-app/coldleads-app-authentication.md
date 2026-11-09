---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coldleads-app-activity-api-openapi.yml
  format: yaml
  label: Cold Leads Activity API
  slug: coldleads-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-activity-api-openapi.yml
- filename: coldleads-app-credits-api-openapi.yml
  format: yaml
  label: Cold Leads Credits API
  slug: coldleads-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-credits-api-openapi.yml
- filename: coldleads-app-find-api-openapi.yml
  format: yaml
  label: Cold Leads Find API
  slug: coldleads-app-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-find-api-openapi.yml
- filename: coldleads-app-follow-ups-api-openapi.yml
  format: yaml
  label: Cold Leads Follow Ups API
  slug: coldleads-app-follow-ups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-follow-ups-api-openapi.yml
- filename: coldleads-app-leads-api-openapi.yml
  format: yaml
  label: Cold Leads Leads API
  slug: coldleads-app-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-leads-api-openapi.yml
- filename: coldleads-app-next-actions-api-openapi.yml
  format: yaml
  label: Cold Leads Next Actions API
  slug: coldleads-app-next-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-next-actions-api-openapi.yml
- filename: coldleads-app-social-api-openapi.yml
  format: yaml
  label: Cold Leads Social API
  slug: coldleads-app-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-social-api-openapi.yml
- filename: coldleads-app-verify-api-openapi.yml
  format: yaml
  label: Cold Leads Verify API
  slug: coldleads-app-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coldleads App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cold Leads secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cold Leads
provider_slug: coldleads-app
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/coldleads-app-openapi.json
  type: apiKey
slug: coldleads-app-authentication
source_filename: coldleads-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/coldleads-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/coldleads-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/coldleads-app/authentication/coldleads-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- Software-as-a-Service
- Small Business
- Lead Management
- Cold Leads
---
