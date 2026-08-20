---
api_key_in:
- header
api_specs:
- filename: amazon-ecs-capacity-providers-api-openapi.yml
  format: yaml
  label: Amazon ECS Capacity Providers API
  slug: amazon-ecs-capacity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-capacity-providers-api-openapi.yml
- filename: amazon-ecs-clusters-api-openapi.yml
  format: yaml
  label: Amazon ECS Clusters API
  slug: amazon-ecs-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-clusters-api-openapi.yml
- filename: amazon-ecs-container-instances-api-openapi.yml
  format: yaml
  label: Amazon ECS Container Instances API
  slug: amazon-ecs-container-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-container-instances-api-openapi.yml
- filename: amazon-ecs-task-definitions-api-openapi.yml
  format: yaml
  label: Amazon ECS Task Definitions API
  slug: amazon-ecs-task-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-task-definitions-api-openapi.yml
- filename: amazon-ecs-tasks-api-openapi.yml
  format: yaml
  label: Amazon ECS Tasks API
  slug: amazon-ecs-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-tasks-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.CreateService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.DeleteService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.DescribeServices API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.ListServices API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.UpdateService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
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
- Containers
- Docker
- ECS
- Orchestration
---
