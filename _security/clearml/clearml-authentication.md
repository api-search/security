---
api_key_in: []
api_specs:
- filename: clearml-openapi.yml
  format: yaml
  label: ClearML REST API
  slug: clearml-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearml/refs/heads/main/openapi/clearml-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clearml Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearML secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClearML
provider_slug: clearml
scheme_count: 2
schemes:
- description: Bearer token obtained from /auth.login
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clearml-openapi.yml
  type: http
- description: HTTP Basic with access_key / secret_key for /auth.login
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/clearml-openapi.yml
  type: http
slug: clearml-authentication
source_filename: clearml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clearml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from /auth.login\n  sources:\n  - openapi/clearml-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with access_key / secret_key for /auth.login\n  sources:\n  - openapi/clearml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearml/refs/heads/main/authentication/clearml-authentication.yml
summary_line: http · 2 schemes
tags:
- ML
- MLOps
- Open Source
- Experiment Tracking
- Orchestration
---
