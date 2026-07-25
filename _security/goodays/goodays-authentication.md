---
api_key_in:
- header
api_specs:
- filename: goodays-core-api-openapi.yml
  format: yaml
  label: Goodays core API
  slug: goodays-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-core-api-openapi.yml
- filename: goodays-dashboard-api-openapi.yml
  format: yaml
  label: Goodays dashboard API
  slug: goodays-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-dashboard-api-openapi.yml
- filename: goodays-events-api-openapi.yml
  format: yaml
  label: Goodays events API
  slug: goodays-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-events-api-openapi.yml
- filename: goodays-response-api-openapi.yml
  format: yaml
  label: Goodays response API
  slug: goodays-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-response-api-openapi.yml
- filename: goodays-session-api-openapi.yml
  format: yaml
  label: Goodays session API
  slug: goodays-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-session-api-openapi.yml
- filename: goodays-solicitation-api-openapi.yml
  format: yaml
  label: Goodays solicitation API
  slug: goodays-solicitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-solicitation-api-openapi.yml
- filename: goodays-stats-api-openapi.yml
  format: yaml
  label: Goodays stats API
  slug: goodays-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-stats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Goodays Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodays secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Goodays
provider_slug: goodays
scheme_count: 1
schemes:
- description: Personal access token supplied verbatim in the Authorization header (no Bearer prefix). Obtain from your Goodays account manager.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/goodays-openapi-original.json
  type: apiKey
slug: goodays-authentication
source_filename: goodays-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/goodays-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Personal access token supplied verbatim in the Authorization header (no Bearer\n    prefix). Obtain from your Goodays account manager.\n  sources:\n  - openapi/goodays-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/authentication/goodays-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Experience
- Customer Feedback
- Voice of the Customer
- Surveys
- NPS
- Reviews
- Retail
- CRM
- SaaS
---
