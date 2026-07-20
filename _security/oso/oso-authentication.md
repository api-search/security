---
api_key_in: []
api_specs:
- filename: api
  format: yaml
  label: Oso Cloud Authorization API
  slug: oso-cloud-authorization-api
  spec_type: OpenAPI
  url: https://www.osohq.com/docs/reference/api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oso Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oso Cloud
provider_slug: oso
scheme_count: 1
schemes:
- bearerFormat: Bearer [example key]
  description: Requires an API key to access.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/oso-authorization-openapi.yml
  type: http
slug: oso-authentication
source_filename: oso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oso-authorization-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer [example key]\n  description: Requires an API key to access.\n  sources:\n  - openapi/oso-authorization-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/authentication/oso-authentication.yml
summary_line: http · 1 scheme
tags:
- Authorization
- Access Control
- RBAC
- ReBAC
- ABAC
- Permissions
- Policy
- Security
- Identity
---
