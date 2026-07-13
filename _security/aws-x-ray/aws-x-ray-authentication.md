---
api_key_in:
- header
api_specs:
- filename: aws-x-ray-openapi.yml
  format: yaml
  label: AWS X-Ray
  slug: aws-x-ray
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws X Ray Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS X-Ray secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS X-Ray
provider_slug: aws-x-ray
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/aws-x-ray-openapi.yml
  type: apiKey
slug: aws-x-ray-authentication
source_filename: aws-x-ray-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-x-ray-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/aws-x-ray-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/authentication/aws-x-ray-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Debugging
- Distributed Tracing
- Microservices
- Observability
---
