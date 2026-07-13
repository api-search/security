---
api_key_in: []
api_specs:
- filename: doordash-drive-openapi.yml
  format: yaml
  label: DoorDash Drive API
  slug: drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-drive-openapi.yml
- filename: doordash-drive-classic-openapi.yml
  format: yaml
  label: DoorDash Drive Classic API
  slug: drive-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-drive-classic-openapi.yml
- filename: doordash-marketplace-openapi.yml
  format: yaml
  label: DoorDash Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-marketplace-openapi.yml
- filename: doordash-item-management-openapi.yml
  format: yaml
  label: DoorDash Item Management API
  slug: marketplace-item-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-item-management-openapi.yml
- filename: doordash-reporting-openapi.yml
  format: yaml
  label: DoorDash Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-reporting-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doordash Authentication
name_suffix: Authentication
oauth_flows: []
overview: doordash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: doordash
provider_slug: doordash
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token signed with your DoorDash developer credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/doordash-drive-classic-openapi.yml
  - openapi/doordash-drive-openapi.yml
  - openapi/doordash-item-management-openapi.yml
  - openapi/doordash-marketplace-openapi.yml
  - openapi/doordash-reporting-openapi.yml
  type: http
slug: doordash-authentication
source_filename: doordash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doordash-drive-classic-openapi.yml, openapi/doordash-drive-openapi.yml, openapi/doordash-item-management-openapi.yml,\n  openapi/doordash-marketplace-openapi.yml, openapi/doordash-reporting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token signed with your DoorDash developer credentials.\n  sources:\n  - openapi/doordash-drive-classic-openapi.yml\n  - openapi/doordash-drive-openapi.yml\n  - openapi/doordash-item-management-openapi.yml\n  - openapi/doordash-marketplace-openapi.yml\n  - openapi/doordash-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/authentication/doordash-authentication.yml
summary_line: http · 1 scheme
tags: []
---
