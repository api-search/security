---
api_key_in:
- header
api_specs:
- filename: aws-s3-openapi.yaml
  format: yaml
  label: Amazon S3 REST API
  slug: amazon-s3-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/openapi/aws-s3-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws S3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon S3 API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon S3 API
provider_slug: aws-s3
scheme_count: 1
schemes:
- description: Amazon S3 signature
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-s3-openapi.yaml
  type: apiKey
slug: aws-s3-authentication
source_filename: aws-s3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-s3-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon S3 signature\n  sources:\n  - openapi/aws-s3-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/authentication/aws-s3-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Storage
- Object Storage
- Storage
---
