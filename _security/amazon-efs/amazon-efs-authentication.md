---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-efs-mount-targets-api-openapi.yml
  format: yaml
  label: Amazon EFS Mount Targets API
  slug: amazon-efs-mount-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-mount-targets-api-openapi.yml
- filename: amazon-efs-filesystems-api-openapi.yml
  format: yaml
  label: Amazon EFS Filesystems API
  slug: amazon-efs-filesystems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-filesystems-api-openapi.yml
- filename: amazon-efs-access-points-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Access Points API
  slug: amazon-efs-access-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-access-points-api-openapi.yml
- filename: amazon-efs-operations-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Operations API
  slug: amazon-efs-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-operations-api-openapi.yml
- filename: amazon-efs-policy-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Policy API
  slug: amazon-efs-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-policy-api-openapi.yml
- filename: amazon-efs-resource-tags-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Resource Tags API
  slug: amazon-efs-resource-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-resource-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/amazon-efs/authentication/amazon-efs-authentication.yml
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
