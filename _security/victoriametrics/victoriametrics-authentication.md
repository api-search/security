---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Victoriametrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: VictoriaMetrics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VictoriaMetrics
provider_slug: victoriametrics
scheme_count: 1
schemes:
- description: Optional HTTP Basic auth when fronted by vmauth
  name: basic
  scheme: basic
  sources:
  - openapi/victoriametrics-openapi.yml
  type: http
slug: victoriametrics-authentication
source_filename: victoriametrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/victoriametrics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Optional HTTP Basic auth when fronted by vmauth\n  sources:\n  - openapi/victoriametrics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoriametrics/refs/heads/main/authentication/victoriametrics-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Time-Series
- Monitoring
- Open Source
- Prometheus
- PromQL
- MetricsQL
- Observability
---
