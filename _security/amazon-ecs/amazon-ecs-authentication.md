---
api_key_in:
- header
api_specs:
- filename: amazon-ecs-openapi.yml
  format: yaml
  label: Amazon ECS API
  slug: amazon-ecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ecs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon ECS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon ECS
provider_slug: amazon-ecs
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-ecs-openapi.yml
  type: apiKey
slug: amazon-ecs-authentication
source_filename: amazon-ecs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ecs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-ecs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/authentication/amazon-ecs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
---
