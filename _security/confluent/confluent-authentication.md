---
api_key_in: []
api_specs:
- filename: confluent-openapi.yml
  format: yaml
  label: Confluent
  slug: confluent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent/refs/heads/main/openapi/confluent-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Confluent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confluent secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Confluent
provider_slug: confluent
scheme_count: 2
schemes:
- description: HTTP Basic authentication using a Confluent Cloud API key (ID:secret)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/confluent-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer token (Confluent STS, external OAuth, or partner token)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/confluent-openapi.yml
  type: http
slug: confluent-authentication
source_filename: confluent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/confluent-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a Confluent Cloud API key (ID:secret)\n  sources:\n  - openapi/confluent-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token (Confluent STS, external OAuth, or partner token)\n  sources:\n  - openapi/confluent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent/refs/heads/main/authentication/confluent-authentication.yml
summary_line: http · 2 schemes
tags: []
---
