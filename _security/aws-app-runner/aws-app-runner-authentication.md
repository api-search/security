---
api_key_in:
- header
api_specs:
- filename: aws-app-runner-openapi.yml
  format: yaml
  label: AWS App Runner
  slug: aws-app-runner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws App Runner Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS App Runner secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS App Runner
provider_slug: aws-app-runner
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/aws-app-runner-openapi.yml
  type: apiKey
slug: aws-app-runner-authentication
source_filename: aws-app-runner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-app-runner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/aws-app-runner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/authentication/aws-app-runner-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
---
