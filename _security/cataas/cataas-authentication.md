---
api_key_in: []
api_specs:
- filename: cataas-admin-api-openapi.yml
  format: yaml
  label: Cataas Admin API
  slug: cataas-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-admin-api-openapi.yml
- filename: cataas-catalog-api-openapi.yml
  format: yaml
  label: Cataas Catalog API
  slug: cataas-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-catalog-api-openapi.yml
- filename: cataas-cats-api-openapi.yml
  format: yaml
  label: Cataas Cats API
  slug: cataas-cats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-cats-api-openapi.yml
- filename: cataas-upload-api-openapi.yml
  format: yaml
  label: Cataas Upload API
  slug: cataas-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-upload-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cataas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cataas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cataas
provider_slug: cataas
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Admin-only bearer token for moderation and catalog management.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cataas-openapi-original.yml
  type: http
slug: cataas-authentication
source_filename: cataas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cataas-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Admin-only bearer token for moderation and catalog management.\n  sources:\n  - openapi/cataas-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/authentication/cataas-authentication.yml
summary_line: http · 1 scheme
tags:
- Animals
- Cats
- Image
- Open-Source
- Public APIs
---
