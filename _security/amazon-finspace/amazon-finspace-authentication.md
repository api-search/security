---
api_key_in:
- header
api_specs:
- filename: amazon-finspace-openapi.yml
  format: yaml
  label: Amazon FinSpace API
  slug: amazon-finspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/openapi/amazon-finspace-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Finspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon FinSpace secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_signature_v4
  parameter: Authorization
  sources:
  - openapi/amazon-finspace-openapi.yml
  type: apiKey
slug: amazon-finspace-authentication
source_filename: amazon-finspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-finspace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-finspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/authentication/amazon-finspace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
---
