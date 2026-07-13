---
api_key_in: []
api_specs:
- filename: apptainer-openapi.yaml
  format: yaml
  label: Apptainer API
  slug: apptainer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptainer/refs/heads/main/openapi/apptainer-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apptainer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptainer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apptainer
provider_slug: apptainer
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apptainer-openapi.yaml
  type: http
slug: apptainer-authentication
source_filename: apptainer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apptainer-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/apptainer-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptainer/refs/heads/main/authentication/apptainer-authentication.yml
summary_line: http · 1 scheme
tags:
- Containers
- HPC
- Scientific Computing
- Open Source
- Linux Foundation
---
