---
api_key_in: []
api_specs:
- filename: delighted-autopilot-api-openapi.yml
  format: yaml
  label: Delighted Autopilot API
  slug: delighted-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-autopilot-api-openapi.yml
- filename: delighted-bounces-api-openapi.yml
  format: yaml
  label: Delighted Bounces API
  slug: delighted-bounces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-bounces-api-openapi.yml
- filename: delighted-metrics-api-openapi.yml
  format: yaml
  label: Delighted Metrics API
  slug: delighted-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-metrics-api-openapi.yml
- filename: delighted-people-api-openapi.yml
  format: yaml
  label: Delighted People API
  slug: delighted-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-people-api-openapi.yml
- filename: delighted-survey-responses-api-openapi.yml
  format: yaml
  label: Delighted Survey Responses API
  slug: delighted-survey-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-survey-responses-api-openapi.yml
- filename: delighted-unsubscribes-api-openapi.yml
  format: yaml
  label: Delighted Unsubscribes API
  slug: delighted-unsubscribes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-unsubscribes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Delighted Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delighted secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delighted
provider_slug: delighted
scheme_count: 1
schemes:
- description: Use your Delighted API key as the username. Leave the password empty. The API key is found in your project settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/delighted-delighted-api-openapi.yml
  type: http
slug: delighted-authentication
source_filename: delighted-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/delighted-delighted-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your Delighted API key as the username. Leave the password empty. The API\n    key is found in your project settings.\n  sources:\n  - openapi/delighted-delighted-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/authentication/delighted-authentication.yml
summary_line: http · 1 scheme
tags:
- NPS
- CSAT
- Customer Satisfaction
- CES
- Customer Effort Score
- Survey
- Customer Experience
- Feedback
- eNPS
---
