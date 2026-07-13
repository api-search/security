---
api_key_in: []
api_specs:
- filename: microsoft-sharepoint-openapi.yml
  format: yaml
  label: SharePoint REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sharepoint/refs/heads/main/openapi/microsoft-sharepoint-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Sharepoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft SharePoint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft SharePoint
provider_slug: microsoft-sharepoint
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-sharepoint-openapi.yml
  type: http
slug: microsoft-sharepoint-authentication
source_filename: microsoft-sharepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-sharepoint-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-sharepoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sharepoint/refs/heads/main/authentication/microsoft-sharepoint-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Content Management
- Microsoft
- Microsoft 365
- SharePoint
---
