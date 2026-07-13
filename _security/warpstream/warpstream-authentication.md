---
api_key_in:
- header
api_specs:
- filename: warpstream-management-openapi.yml
  format: yaml
  label: WarpStream Management API
  slug: warpstream-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Warpstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: WarpStream secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WarpStream
provider_slug: warpstream
scheme_count: 1
schemes:
- description: 'WarpStream API key. Three key types are supported: Application Keys (manage workspace-specific resources), Agent Keys (scoped to a specific virtual cluster), and Account Keys (manage account-level resources such as workspaces and users).'
  in: header
  name: ApiKeyAuth
  parameter: warpstream-api-key
  sources:
  - openapi/warpstream-management-openapi.yml
  type: apiKey
slug: warpstream-authentication
source_filename: warpstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warpstream-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: warpstream-api-key\n  description: 'WarpStream API key. Three key types are supported: Application Keys (manage\n    workspace-specific resources), Agent Keys (scoped to a specific virtual cluster), and Account\n    Keys (manage account-level resources such as workspaces and users).'\n  sources:\n  - openapi/warpstream-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/authentication/warpstream-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Kafka
- Streaming
- Serverless
- Object Storage
- BYOC
- Data Streaming
- Apache Kafka
- Message Queue
- Event Streaming
---
