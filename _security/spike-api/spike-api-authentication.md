---
api_key_in: []
api_specs:
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Authentication API
  slug: spike-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Integrations API
  slug: spike-api-provider-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Records API
  slug: spike-api-provider-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Sleep API
  slug: spike-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Workouts API
  slug: spike-api-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Time Series API
  slug: spike-api-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Statistics API
  slug: spike-api-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Nutrition AI API
  slug: spike-api-nutrition-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Lab Reports API
  slug: spike-api-lab-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Users API
  slug: spike-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike SDK Push API
  slug: spike-api-sdk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spike Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spike secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spike
provider_slug: spike-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/spike-api-openapi.yml
  type: http
slug: spike-api-authentication
source_filename: spike-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spike-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/spike-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/authentication/spike-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Health Data
- Wearables
- Fitness
- Digital Health
- Data Aggregation
- HIPAA
---
