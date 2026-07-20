---
api_key_in:
- header
api_specs:
- filename: archil-openapi-original.yml
  format: yaml
  label: Archil Control Plane API
  slug: archil-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Archil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archil secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Archil
provider_slug: archil
scheme_count: 1
schemes:
- description: API key
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/archil-openapi-original.yml
  type: apiKey
slug: archil-authentication
source_filename: archil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/archil-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key\n  sources:\n  - openapi/archil-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/authentication/archil-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cloud Storage
- Filesystem
- Object Storage
- Artificial Intelligence
- Infrastructure
- Developer Tools
- Serverless
- Data
- S3
---
