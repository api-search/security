---
api_key_in:
- header
api_specs:
- filename: cubefs-s3-api-openapi.yml
  format: yaml
  label: CubeFS S3-Compatible API
  slug: cubefs-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-s3-api-openapi.yml
- filename: cubefs-master-api-openapi.yml
  format: yaml
  label: CubeFS Master API
  slug: cubefs-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-master-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cubefs Authentication
name_suffix: Authentication
oauth_flows: []
overview: CubeFS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CubeFS
provider_slug: cubefs
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4 authorization. Format: AWS4-HMAC-SHA256 Credential={accessKey}/{date}/{region}/s3/aws4_request, SignedHeaders={headers}, Signature={signature}. Access keys are managed via the CubeFS Master API user management endpoints.'
  in: header
  name: awsAuth
  parameter: Authorization
  sources:
  - openapi/cubefs-s3-api-openapi.yml
  type: apiKey
slug: cubefs-authentication
source_filename: cubefs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cubefs-s3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'AWS Signature Version 4 authorization. Format: AWS4-HMAC-SHA256 Credential={accessKey}/{date}/{region}/s3/aws4_request,\n    SignedHeaders={headers}, Signature={signature}. Access keys are managed via the CubeFS Master\n    API user management endpoints.'\n  sources:\n  - openapi/cubefs-s3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/authentication/cubefs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Native
- CNCF Graduated
- Distributed File System
- Kubernetes
- Object Storage
- POSIX
- S3 Compatible
- Storage
---
