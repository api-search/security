---
api_key_in: []
api_specs:
- filename: timoni-openapi.yml
  format: yaml
  label: Timoni Module Registry API
  slug: timoni
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timoni/refs/heads/main/openapi/timoni-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Timoni Authentication
name_suffix: Authentication
oauth_flows: []
overview: Timoni secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Timoni
provider_slug: timoni
scheme_count: 2
schemes:
- description: OCI registry authentication token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/timoni-openapi.yml
  type: http
- description: Username and password authentication for OCI registry
  name: basicAuth
  scheme: basic
  sources:
  - openapi/timoni-openapi.yml
  type: http
slug: timoni-authentication
source_filename: timoni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/timoni-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OCI registry authentication token\n  sources:\n  - openapi/timoni-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username and password authentication for OCI registry\n  sources:\n  - openapi/timoni-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timoni/refs/heads/main/authentication/timoni-authentication.yml
summary_line: http · 2 schemes
tags:
- Containers
- Kubernetes
- Package Manager
- CUE
---
