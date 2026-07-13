---
api_key_in:
- header
api_specs:
- filename: elastic-observability-openapi.yml
  format: yaml
  label: Elastic Observability
  slug: elastic-observability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Observability Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic Observability secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic Observability
provider_slug: elastic-observability
scheme_count: 2
schemes:
- bearerFormat: Secret token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/elastic-observability-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elastic-observability-openapi.yml
  type: apiKey
slug: elastic-observability-authentication
source_filename: elastic-observability-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elastic-observability-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Secret token\n  sources:\n  - openapi/elastic-observability-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/elastic-observability-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/authentication/elastic-observability-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AIOps
- Observability
---
