---
api_key_in: []
api_specs:
- filename: 6733983cabaf62002c7b16d9
  format: yaml
  label: ReadMe API
  slug: readme-api
  spec_type: OpenAPI
  url: https://spec.readme.com/openapi/6733983cabaf62002c7b16d9
- filename: readme-metrics-openapi.yml
  format: yaml
  label: ReadMe Metrics
  slug: readme-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/openapi/readme-metrics-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Readme Metrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReadMe Metrics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ReadMe Metrics
provider_slug: readme-metrics
scheme_count: 1
schemes:
- description: ReadMe API key supplied as the HTTP Basic username (password empty).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/readme-metrics-openapi.yml
  type: http
slug: readme-metrics-authentication
source_filename: readme-metrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/readme-metrics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: ReadMe API key supplied as the HTTP Basic username (password empty).\n  sources:\n  - openapi/readme-metrics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/authentication/readme-metrics-authentication.yml
summary_line: http · 1 scheme
tags:
- API Analytics
- API Documentation
- API Logs
- API Metrics
- API Usage
- Developer Experience
- Developer Hubs
---
