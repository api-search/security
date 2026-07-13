---
api_key_in:
- header
api_specs:
- filename: amazon-s3-rest-api-openapi.yml
  format: yaml
  label: Amazon S3 REST API
  slug: amazon-s3-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-rest-api-openapi.yml
- filename: amazon-s3-control-api-openapi.yml
  format: yaml
  label: Amazon S3 Control API
  slug: amazon-s3-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-control-api-openapi.yml
- filename: amazon-s3-tables-api-openapi.yml
  format: yaml
  label: Amazon S3 Tables API
  slug: amazon-s3-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-tables-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon S3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon S3 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon S3
provider_slug: amazon-s3
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. The S3 Control API uses the service name s3 for signing.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-s3-control-api-openapi.yml
  - openapi/amazon-s3-rest-api-openapi.yml
  - openapi/amazon-s3-tables-api-openapi.yml
  type: apiKey
slug: amazon-s3-authentication
source_filename: amazon-s3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-s3-control-api-openapi.yml, openapi/amazon-s3-rest-api-openapi.yml, openapi/amazon-s3-tables-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. The S3 Control API uses the service name\n    s3 for signing.\n  sources:\n  - openapi/amazon-s3-control-api-openapi.yml\n  - openapi/amazon-s3-rest-api-openapi.yml\n  - openapi/amazon-s3-tables-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/authentication/amazon-s3-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
---
