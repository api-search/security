---
api_key_in:
- header
api_specs:
- filename: aws-backup-openapi.yml
  format: yaml
  label: AWS Backup API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Backup Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Backup secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Backup
provider_slug: aws-backup
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-backup-openapi.yml
  type: apiKey
slug: aws-backup-authentication
source_filename: aws-backup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-backup-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-backup-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/authentication/aws-backup-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- Data Protection
- Disaster Recovery
- Managed Service
- Compliance
---
