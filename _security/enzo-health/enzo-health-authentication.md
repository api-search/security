---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enzo-health-workflow-runs-api-openapi.yml
  format: yaml
  label: Enzo Health Workflow Runs API
  slug: enzo-health-workflow-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enzo-health/openapi/enzo-health-workflow-runs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Enzo Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enzo Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enzo Health
provider_slug: enzo-health
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/enzo-health-openapi.json
  type: http
slug: enzo-health-authentication
source_filename: enzo-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: derived\nsource: openapi/enzo-health-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/enzo-health-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/enzo-health/authentication/enzo-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Home Health
- EHR
- Healthcare
- SaaS
---
