---
api_key_in:
- header
api_specs:
- filename: fargate-clusters-api-openapi.yml
  format: yaml
  label: AWS Fargate Clusters API
  slug: fargate-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-clusters-api-openapi.yml
- filename: fargate-task-definitions-api-openapi.yml
  format: yaml
  label: AWS Fargate Task Definitions API
  slug: fargate-task-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-task-definitions-api-openapi.yml
- filename: fargate-tasks-api-openapi.yml
  format: yaml
  label: AWS Fargate Tasks API
  slug: fargate-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-tasks-api-openapi.yml
- filename: fargate-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
  format: yaml
  label: 'AWS Fargate #X Amz Target=AmazonEC2ContainerServiceV20141113.CreateService API'
  slug: fargate-x-amz-target-amazonec2containerservicev20141113-createservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
- filename: fargate-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
  format: yaml
  label: 'AWS Fargate #X Amz Target=AmazonEC2ContainerServiceV20141113.DeleteService API'
  slug: fargate-x-amz-target-amazonec2containerservicev20141113-deleteservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
- filename: fargate-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
  format: yaml
  label: 'AWS Fargate #X Amz Target=AmazonEC2ContainerServiceV20141113.DescribeServices API'
  slug: fargate-x-amz-target-amazonec2containerservicev20141113-describeservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
- filename: fargate-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
  format: yaml
  label: 'AWS Fargate #X Amz Target=AmazonEC2ContainerServiceV20141113.ListServices API'
  slug: fargate-x-amz-target-amazonec2containerservicev20141113-listservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
- filename: fargate-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
  format: yaml
  label: 'AWS Fargate #X Amz Target=AmazonEC2ContainerServiceV20141113.UpdateService API'
  slug: fargate-x-amz-target-amazonec2containerservicev20141113-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/openapi/fargate-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
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
