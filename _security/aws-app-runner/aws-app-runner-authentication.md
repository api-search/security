---
api_key_in:
- header
api_specs:
- filename: aws-app-runner-auto-scaling-api-openapi.yml
  format: yaml
  label: AWS App Runner Auto Scaling API
  slug: aws-app-runner-auto-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-auto-scaling-api-openapi.yml
- filename: aws-app-runner-aws-app-runner-api-api-openapi.yml
  format: yaml
  label: AWS App Runner AWS App Runner API API
  slug: aws-app-runner-aws-app-runner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-aws-app-runner-api-api-openapi.yml
- filename: aws-app-runner-connections-api-openapi.yml
  format: yaml
  label: AWS App Runner Connections API
  slug: aws-app-runner-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-connections-api-openapi.yml
- filename: aws-app-runner-custom-domains-api-openapi.yml
  format: yaml
  label: AWS App Runner Custom Domains API
  slug: aws-app-runner-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-custom-domains-api-openapi.yml
- filename: aws-app-runner-deleteservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #DeleteService API'
  slug: aws-app-runner-deleteservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-deleteservice-api-openapi.yml
- filename: aws-app-runner-deployments-api-openapi.yml
  format: yaml
  label: AWS App Runner Deployments API
  slug: aws-app-runner-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-deployments-api-openapi.yml
- filename: aws-app-runner-describeservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #DescribeService API'
  slug: aws-app-runner-describeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-describeservice-api-openapi.yml
- filename: aws-app-runner-listservices-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #ListServices API'
  slug: aws-app-runner-listservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-listservices-api-openapi.yml
- filename: aws-app-runner-observability-api-openapi.yml
  format: yaml
  label: AWS App Runner Observability API
  slug: aws-app-runner-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-observability-api-openapi.yml
- filename: aws-app-runner-pauseservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #PauseService API'
  slug: aws-app-runner-pauseservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-pauseservice-api-openapi.yml
- filename: aws-app-runner-resumeservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #ResumeService API'
  slug: aws-app-runner-resumeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-resumeservice-api-openapi.yml
- filename: aws-app-runner-updateservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #UpdateService API'
  slug: aws-app-runner-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-updateservice-api-openapi.yml
- filename: aws-app-runner-vpc-api-openapi.yml
  format: yaml
  label: AWS App Runner VPC API
  slug: aws-app-runner-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-vpc-api-openapi.yml
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
