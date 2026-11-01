---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alloy-automation-credentials-api-openapi.yml
  format: yaml
  label: Alloy Automation Credentials API
  slug: alloy-automation-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-credentials-api-openapi.yml
- filename: alloy-automation-events-api-openapi.yml
  format: yaml
  label: Alloy Automation Events API
  slug: alloy-automation-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-events-api-openapi.yml
- filename: alloy-automation-integrations-api-openapi.yml
  format: yaml
  label: Alloy Automation Integrations API
  slug: alloy-automation-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-integrations-api-openapi.yml
- filename: alloy-automation-passthrough-api-openapi.yml
  format: yaml
  label: Alloy Automation Passthrough API
  slug: alloy-automation-passthrough-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-passthrough-api-openapi.yml
- filename: alloy-automation-users-api-openapi.yml
  format: yaml
  label: Alloy Automation Users API
  slug: alloy-automation-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-users-api-openapi.yml
- filename: alloy-automation-analytics-api-openapi.yml
  format: yaml
  label: Alloy Automation Analytics API
  slug: alloy-automation-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-analytics-api-openapi.yml
- filename: alloy-automation-headless-api-openapi.yml
  format: yaml
  label: Alloy Automation Headless API
  slug: alloy-automation-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-headless-api-openapi.yml
- filename: alloy-automation-installations-api-openapi.yml
  format: yaml
  label: Alloy Automation Installations API
  slug: alloy-automation-installations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-installations-api-openapi.yml
- filename: alloy-automation-logs-api-openapi.yml
  format: yaml
  label: Alloy Automation Logs API
  slug: alloy-automation-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-logs-api-openapi.yml
- filename: alloy-automation-metadata-api-openapi.yml
  format: yaml
  label: Alloy Automation Metadata API
  slug: alloy-automation-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-metadata-api-openapi.yml
- filename: alloy-automation-run-api-openapi.yml
  format: yaml
  label: Alloy Automation Run API
  slug: alloy-automation-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-run-api-openapi.yml
- filename: alloy-automation-workflows-api-openapi.yml
  format: yaml
  label: Alloy Automation Workflows API
  slug: alloy-automation-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-automation/openapi/alloy-automation-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Alloy Automation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloy Automation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alloy Automation
provider_slug: alloy-automation
scheme_count: 1
schemes:
- description: 'Bearer API key in the Authorization header, e.g. `Authorization: Bearer [example key]`. Frontend calls use a per-user JWT instead of the master key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alloy-automation-openapi.yml
  type: http
slug: alloy-automation-authentication
source_filename: alloy-automation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-automation-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key in the Authorization header, e.g. `Authorization: Bearer [example key]`.\n    Frontend calls use a per-user JWT instead of the master key.'\n  sources:\n  - openapi/alloy-automation-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/alloy-automation/authentication/alloy-automation-authentication.yml
summary_line: http · 1 scheme
tags:
- iPaaS
- Integration
- Unified API
- Embedded
- Software-as-a-Service
- Automation
---
