---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codepipeline-executions-api-openapi.yml
  format: yaml
  label: Amazon CodePipeline Executions API
  slug: amazon-codepipeline-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/openapi/amazon-codepipeline-executions-api-openapi.yml
- filename: amazon-codepipeline-pipelines-api-openapi.yml
  format: yaml
  label: Amazon CodePipeline Pipelines API
  slug: amazon-codepipeline-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/openapi/amazon-codepipeline-pipelines-api-openapi.yml
- filename: amazon-codepipeline-aws-codepipeline-api-openapi.yml
  format: yaml
  label: Amazon CodePipeline AWS CodePipeline API
  slug: amazon-codepipeline-aws-codepipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/openapi/amazon-codepipeline-aws-codepipeline-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Codepipeline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodePipeline secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codepipeline-openapi-original.yaml
  type: apiKey
slug: amazon-codepipeline-authentication
source_filename: amazon-codepipeline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codepipeline-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codepipeline-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/authentication/amazon-codepipeline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- CI/CD
- Continuous Delivery
- Developer Tools
- DevOps
- Pipelines
- Release Automation
---
