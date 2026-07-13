---
api_key_in:
- header
api_specs:
- filename: amazon-storage-gateway.yaml
  format: yaml
  label: Amazon Storage Gateway REST API
  slug: amazon-storage-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/openapi/amazon-storage-gateway.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Storage Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Storage Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-storage-gateway-api-openapi.yml
  - openapi/amazon-storage-gateway.yaml
  type: apiKey
slug: amazon-storage-gateway-authentication
source_filename: amazon-storage-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-storage-gateway-api-openapi.yml, openapi/amazon-storage-gateway.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-storage-gateway-api-openapi.yml\n  - openapi/amazon-storage-gateway.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/authentication/amazon-storage-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
---
