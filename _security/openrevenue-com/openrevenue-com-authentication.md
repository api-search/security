---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openrevenue-com-account-api-openapi.yml
  format: yaml
  label: OpenRevenue Account API
  slug: openrevenue-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-account-api-openapi.yml
- filename: openrevenue-com-analytics-api-openapi.yml
  format: yaml
  label: OpenRevenue Analytics API
  slug: openrevenue-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-analytics-api-openapi.yml
- filename: openrevenue-com-funnels-api-openapi.yml
  format: yaml
  label: OpenRevenue Funnels API
  slug: openrevenue-com-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-funnels-api-openapi.yml
- filename: openrevenue-com-performance-api-openapi.yml
  format: yaml
  label: OpenRevenue Performance API
  slug: openrevenue-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-performance-api-openapi.yml
- filename: openrevenue-com-visitors-api-openapi.yml
  format: yaml
  label: OpenRevenue Visitors API
  slug: openrevenue-com-visitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-visitors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: OpenRevenue Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRevenue secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRevenue
provider_slug: openrevenue-com
scheme_count: 1
schemes:
- bearerFormat: openrevenue_…
  description: Account API key from Account → API. Use a read-only key for analytics; write is required to create or delete projects.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openrevenue-com-openapi.json
  type: http
slug: openrevenue-com-authentication
source_filename: openrevenue-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/openrevenue-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: openrevenue_…\n  description: Account API key from Account → API. Use a read-only key for analytics; write\n    is required to create or delete projects.\n  sources:\n  - openapi/openrevenue-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/openrevenue-com/authentication/openrevenue-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web
- Privacy
- Revenue
- Marketing
- Company
---
