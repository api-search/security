---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: Cerbos PDP REST API
  slug: cerbos-pdp-rest-api
  spec_type: OpenAPI
  url: https://docs.cerbos.dev/cerbos/latest/api/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cerbos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerbos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cerbos
provider_slug: cerbos
scheme_count: 1
schemes:
- description: Basic authentication for the Admin API (default cerbos/cerbosAdmin; override in production).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cerbos-openapi.yml
  type: http
slug: cerbos-authentication
source_filename: cerbos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cerbos-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication for the Admin API (default cerbos/cerbosAdmin; override\n    in production).\n  sources:\n  - openapi/cerbos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/authentication/cerbos-authentication.yml
summary_line: http · 1 scheme
tags:
- ABAC
- Access Control
- Authorization
- AuthZEN
- Open Source
- PBAC
- PDP
- Permissions
- Policy as Code
- RBAC
- ReBAC
- Zero Trust
---
