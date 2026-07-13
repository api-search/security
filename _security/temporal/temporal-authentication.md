---
api_key_in: []
api_specs:
- filename: cloud-ops-api.yml
  format: yaml
  label: Temporal Cloud Ops API
  slug: cloud-ops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/cloud-ops-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Temporal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temporal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Temporal
provider_slug: temporal
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-ops-api.yml
  type: http
slug: temporal-authentication
source_filename: temporal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-ops-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/cloud-ops-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/authentication/temporal-authentication.yml
summary_line: http · 1 scheme
tags:
- ProCode_API_Composition
- Workflows
---
