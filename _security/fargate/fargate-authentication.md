---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon ECS API (Fargate)
  slug: amazon-ecs-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/ecs/2014-11-13/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon EKS API (Fargate)
  slug: amazon-eks-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/eks/2017-11-01/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fargate Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Fargate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Fargate
provider_slug: fargate
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed using AWS access credentials.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/fargate-ecs-openapi.yml
  type: apiKey
slug: fargate-authentication
source_filename: fargate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fargate-ecs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Requests must be signed using AWS access\n    credentials.\n  sources:\n  - openapi/fargate-ecs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/authentication/fargate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Containers
- Docker
- Kubernetes
- Serverless
---
