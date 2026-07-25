---
api_key_in: []
api_specs:
- filename: cerbos-authzen-api-openapi.yml
  format: yaml
  label: Cerbos AuthZEN API
  slug: cerbos-authzen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-authzen-api-openapi.yml
- filename: cerbos-admin-audit-api-openapi.yml
  format: yaml
  label: Cerbos Admin Audit API
  slug: cerbos-admin-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-admin-audit-api-openapi.yml
- filename: cerbos-admin-policies-api-openapi.yml
  format: yaml
  label: Cerbos Admin Policies API
  slug: cerbos-admin-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-admin-policies-api-openapi.yml
- filename: cerbos-admin-schemas-api-openapi.yml
  format: yaml
  label: Cerbos Admin Schemas API
  slug: cerbos-admin-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-admin-schemas-api-openapi.yml
- filename: cerbos-admin-store-api-openapi.yml
  format: yaml
  label: Cerbos Admin Store API
  slug: cerbos-admin-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-admin-store-api-openapi.yml
- filename: cerbos-authzen-api-openapi.yml
  format: yaml
  label: Cerbos AuthZEN API
  slug: cerbos-authzen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-authzen-api-openapi.yml
- filename: cerbos-check-api-openapi.yml
  format: yaml
  label: Cerbos Check API
  slug: cerbos-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-check-api-openapi.yml
- filename: cerbos-plan-api-openapi.yml
  format: yaml
  label: Cerbos Plan API
  slug: cerbos-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-plan-api-openapi.yml
- filename: cerbos-server-api-openapi.yml
  format: yaml
  label: Cerbos Server API
  slug: cerbos-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/openapi/cerbos-server-api-openapi.yml
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
