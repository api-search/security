---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Resource Explorer API
  slug: aws-resource-explorer-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/resource-explorer-2/2022-07-28/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Resource Explorer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Resource Explorer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-resource-explorer-openapi.yml
  type: apiKey
slug: amazon-resource-explorer-authentication
source_filename: amazon-resource-explorer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-resource-explorer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-resource-explorer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/authentication/amazon-resource-explorer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Discovery
- Inventory
- Operations
- Resource Management
---
