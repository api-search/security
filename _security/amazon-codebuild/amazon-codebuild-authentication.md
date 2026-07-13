---
api_key_in:
- header
api_specs:
- filename: amazon-codebuild-openapi-original.yaml
  format: yaml
  label: Amazon CodeBuild API
  slug: amazon-codebuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/openapi/amazon-codebuild-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Codebuild Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeBuild secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codebuild-openapi-original.yaml
  type: apiKey
slug: amazon-codebuild-authentication
source_filename: amazon-codebuild-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codebuild-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codebuild-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/authentication/amazon-codebuild-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
---
