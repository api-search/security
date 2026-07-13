---
api_key_in: []
api_specs:
- filename: drone-ci-openapi.yml
  format: yaml
  label: Drone Server REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone-ci/refs/heads/main/openapi/drone-ci-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drone Ci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drone
provider_slug: drone-ci
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drone-ci-openapi.yml
  type: http
slug: drone-ci-authentication
source_filename: drone-ci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drone-ci-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/drone-ci-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone-ci/refs/heads/main/authentication/drone-ci-authentication.yml
summary_line: http · 1 scheme
tags:
- DevOps
- CI/CD
- Container-Native
- Open Source
- YAML
- Harness
---
