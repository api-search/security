---
api_key_in:
- header
api_specs:
- filename: amazon-s3-glacier-openapi.yml
  format: yaml
  label: Amazon S3 Glacier API
  slug: amazon-s3-glacier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/openapi/amazon-s3-glacier-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon S3 Glacier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon S3 Glacier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-s3-glacier-api-openapi.yml
  type: apiKey
slug: amazon-s3-glacier-authentication
source_filename: amazon-s3-glacier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-s3-glacier-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-s3-glacier-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/authentication/amazon-s3-glacier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Archive
- Backup
- Storage
---
