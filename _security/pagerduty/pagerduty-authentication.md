---
api_key_in:
- header
api_specs:
- filename: pagerduty-openapi-original.yml
  format: yaml
  label: PagerDuty REST API
  slug: pagerduty-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/openapi/pagerduty-openapi-original.yml
- filename: pagerduty-events-asyncapi.yml
  format: yaml
  label: PagerDuty Events API
  slug: pagerduty-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/asyncapi/pagerduty-events-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pagerduty Authentication
name_suffix: Authentication
oauth_flows: []
overview: PagerDuty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PagerDuty
provider_slug: pagerduty
scheme_count: 1
schemes:
- description: The API Key with format `Token token=<API_KEY>`
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/pagerduty-openapi-original.yml
  type: apiKey
slug: pagerduty-authentication
source_filename: pagerduty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pagerduty-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The API Key with format `Token token=<API_KEY>`\n  sources:\n  - openapi/pagerduty-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/authentication/pagerduty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alerting
- DevOps
- Incident Management
- On-Call Management
---
