---
api_key_in:
- header
api_specs:
- filename: aws-codebuild-openapi.yml
  format: yaml
  label: AWS CodeBuild API
  slug: codebuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Codebuild Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS CodeBuild secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS CodeBuild
provider_slug: aws-codebuild
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-codebuild-openapi.yml
  type: apiKey
slug: aws-codebuild-authentication
source_filename: aws-codebuild-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-codebuild-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-codebuild-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/authentication/aws-codebuild-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Build
- CI/CD
- Continuous Integration
- Developer Tools
- DevOps
---
