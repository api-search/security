---
api_key_in:
- query
api_specs:
- filename: airbrake-activities-api-openapi.yml
  format: yaml
  label: Airbrake Activities API
  slug: airbrake-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-activities-api-openapi.yml
- filename: airbrake-deploys-api-openapi.yml
  format: yaml
  label: Airbrake Deploys API
  slug: airbrake-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-deploys-api-openapi.yml
- filename: airbrake-groups-api-openapi.yml
  format: yaml
  label: Airbrake Groups API
  slug: airbrake-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-groups-api-openapi.yml
- filename: airbrake-ios-crash-reports-api-openapi.yml
  format: yaml
  label: Airbrake iOS Crash Reports API
  slug: airbrake-ios-crash-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-ios-crash-reports-api-openapi.yml
- filename: airbrake-notices-api-openapi.yml
  format: yaml
  label: Airbrake Notices API
  slug: airbrake-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-notices-api-openapi.yml
- filename: airbrake-performance-api-openapi.yml
  format: yaml
  label: Airbrake Performance API
  slug: airbrake-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-performance-api-openapi.yml
- filename: airbrake-projects-api-openapi.yml
  format: yaml
  label: Airbrake Projects API
  slug: airbrake-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-projects-api-openapi.yml
- filename: airbrake-sessions-api-openapi.yml
  format: yaml
  label: Airbrake Sessions API
  slug: airbrake-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-sessions-api-openapi.yml
- filename: airbrake-source-maps-api-openapi.yml
  format: yaml
  label: Airbrake Source Maps API
  slug: airbrake-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-source-maps-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airbrake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airbrake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airbrake
provider_slug: airbrake
scheme_count: 1
schemes:
- description: Project key, user key, or user token passed as the `key` query string parameter.
  in: query
  name: ProjectKey
  parameter: key
  sources:
  - openapi/airbrake-openapi.yml
  type: apiKey
slug: airbrake-authentication
source_filename: airbrake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airbrake-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ProjectKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Project key, user key, or user token passed as the `key` query string parameter.\n  sources:\n  - openapi/airbrake-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/authentication/airbrake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Error Monitoring
- Application Performance Monitoring
- Observability
- DevOps
- Logging
- Exception Tracking
---
