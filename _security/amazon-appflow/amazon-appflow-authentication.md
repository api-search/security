---
api_key_in:
- header
api_specs:
- filename: amazon-appflow-openapi.yml
  format: yaml
  label: Amazon AppFlow API
  slug: amazon-appflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/openapi/amazon-appflow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Appflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon AppFlow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-appflow-openapi.yml
  type: apiKey
slug: amazon-appflow-authentication
source_filename: amazon-appflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-appflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-appflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/authentication/amazon-appflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
---
