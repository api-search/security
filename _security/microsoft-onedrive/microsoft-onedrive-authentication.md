---
api_key_in: []
api_specs:
- filename: microsoft-onedrive-openapi.yml
  format: yaml
  label: Microsoft Graph OneDrive API
  slug: graph-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onedrive/refs/heads/main/openapi/microsoft-onedrive-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Onedrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft OneDrive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft OneDrive
provider_slug: microsoft-onedrive
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-onedrive-openapi.yml
  type: http
slug: microsoft-onedrive-authentication
source_filename: microsoft-onedrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-onedrive-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-onedrive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-onedrive/refs/heads/main/authentication/microsoft-onedrive-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Storage
- File Storage
- Files
- Microsoft
- Microsoft 365
---
