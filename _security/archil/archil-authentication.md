---
api_key_in:
- header
api_specs:
- filename: archil-api-tokens-api-openapi.yml
  format: yaml
  label: Archil API Tokens API
  slug: archil-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-api-tokens-api-openapi.yml
- filename: archil-disk-users-api-openapi.yml
  format: yaml
  label: Archil Disk Users API
  slug: archil-disk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-disk-users-api-openapi.yml
- filename: archil-disks-api-openapi.yml
  format: yaml
  label: Archil Disks API
  slug: archil-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-disks-api-openapi.yml
- filename: archil-serverless-execution-api-openapi.yml
  format: yaml
  label: Archil Serverless Execution API
  slug: archil-serverless-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-serverless-execution-api-openapi.yml
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
