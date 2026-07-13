---
api_key_in:
- header
api_specs:
- filename: north-cloud-openapi.yml
  format: yaml
  label: North.Cloud Public API
  slug: north-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/openapi/north-cloud-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: North Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: North.Cloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: North.Cloud
provider_slug: north-cloud
scheme_count: 1
schemes:
- description: Provide the API key as `ApiKey north_api_{your_key}`. Keys are created in Streams -> API Keys within the North.Cloud application.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/north-cloud-openapi.yml
  type: apiKey
slug: north-cloud-authentication
source_filename: north-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/north-cloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide the API key as `ApiKey north_api_{your_key}`. Keys are created in Streams\n    -> API Keys within the North.Cloud application.\n  sources:\n  - openapi/north-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/authentication/north-cloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FinOps
- Cloud Cost Management
- GCP
- Cost Optimization
- Cost Units
---
