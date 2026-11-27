---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findefend-com-alerts-api-openapi.yml
  format: yaml
  label: FinDefend Alerts API
  slug: findefend-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-alerts-api-openapi.yml
- filename: findefend-com-export-api-openapi.yml
  format: yaml
  label: FinDefend Export API
  slug: findefend-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-export-api-openapi.yml
- filename: findefend-com-health-api-openapi.yml
  format: yaml
  label: FinDefend Health API
  slug: findefend-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-health-api-openapi.yml
- filename: findefend-com-summary-api-openapi.yml
  format: yaml
  label: FinDefend Summary API
  slug: findefend-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-summary-api-openapi.yml
- filename: findefend-com-vendors-api-openapi.yml
  format: yaml
  label: FinDefend Vendors API
  slug: findefend-com-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FinDefend Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinDefend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FinDefend
provider_slug: findefend-com
scheme_count: 1
schemes:
- description: 'User API key minted at /app/settings (fd_…). Scopes: read (GETs), write (PATCH/POST).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/findefend-com-openapi.yml
  type: http
slug: findefend-com-authentication
source_filename: findefend-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/findefend-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'User API key minted at /app/settings (fd_…). Scopes: read (GETs), write (PATCH/POST).'\n  sources:\n  - openapi/findefend-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/findefend-com/authentication/findefend-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Software-as-a-Service
- Subscription Management
- Expense Tracking
- Automation
---
