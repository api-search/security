---
api_key_in: []
api_specs:
- filename: datocms-content-management-api.yml
  format: yaml
  label: DatoCMS Content Management API
  slug: datocms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-content-management-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datocms Authentication
name_suffix: Authentication
oauth_flows: []
overview: DatoCMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DatoCMS
provider_slug: datocms
scheme_count: 1
schemes:
- bearerFormat: API token
  name: apiTokenAuth
  scheme: bearer
  sources:
  - openapi/datocms-content-management-api.yml
  type: http
slug: datocms-authentication
source_filename: datocms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datocms-content-management-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API token\n  sources:\n  - openapi/datocms-content-management-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/authentication/datocms-authentication.yml
summary_line: http · 1 scheme
tags:
- CMS
- Content Delivery
- Content Management
- GraphQL
- Headless CMS
---
