---
api_key_in: []
api_specs:
- filename: oso-centralized-authorization-data-api-openapi.yml
  format: yaml
  label: Oso Cloud Centralized Authorization Data API
  slug: oso-centralized-authorization-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/openapi/oso-centralized-authorization-data-api-openapi.yml
- filename: oso-check-api-api-openapi.yml
  format: yaml
  label: Oso Cloud Check API API
  slug: oso-check-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/openapi/oso-check-api-api-openapi.yml
- filename: oso-local-check-api-api-openapi.yml
  format: yaml
  label: Oso Cloud Local Check API API
  slug: oso-local-check-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/openapi/oso-local-check-api-api-openapi.yml
- filename: oso-policy-api-openapi.yml
  format: yaml
  label: Oso Cloud Policy API
  slug: oso-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/openapi/oso-policy-api-openapi.yml
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
