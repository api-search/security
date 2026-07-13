---
api_key_in:
- header
api_specs:
- filename: amazon-efs-openapi.yml
  format: yaml
  label: Amazon EFS API
  slug: amazon-efs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/openapi/amazon-efs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Efs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EFS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EFS
provider_slug: amazon-efs
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-efs-openapi.yml
  type: apiKey
slug: amazon-efs-authentication
source_filename: amazon-efs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-efs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-efs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/authentication/amazon-efs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
---
