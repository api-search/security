---
api_key_in: []
api_specs:
- filename: appsmith-openapi.yaml
  format: yaml
  label: Appsmith API
  slug: appsmith-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/openapi/appsmith-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appsmith secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appsmith
provider_slug: appsmith
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appsmith-openapi.yaml
  type: http
slug: appsmith-authentication
source_filename: appsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appsmith-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/appsmith-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/authentication/appsmith-authentication.yml
summary_line: http · 1 scheme
tags:
- Low-Code
- Open Source
- Internal Tools
- Workflow Automation
- Developer Tools
---
