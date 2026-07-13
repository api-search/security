---
api_key_in:
- header
api_specs:
- filename: amazon-rds-openapi.yml
  format: yaml
  label: Amazon RDS API
  slug: amazon-rds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/openapi/amazon-rds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Rds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon RDS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon RDS
provider_slug: amazon-rds
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-rds-openapi.yml
  type: apiKey
slug: amazon-rds-authentication
source_filename: amazon-rds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-rds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-rds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/authentication/amazon-rds-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
---
