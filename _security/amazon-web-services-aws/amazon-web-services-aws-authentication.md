---
api_key_in:
- header
api_specs:
- filename: amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
  format: yaml
  label: Amazon Web Services (AWS) Amazon EC2 API API
  slug: amazon-web-services-aws-amazon-ec2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Web Services Aws Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Web Services (AWS) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Web Services (AWS)
provider_slug: amazon-web-services-aws
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request.
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/amazon-web-services-aws-openapi.yml
  type: apiKey
slug: amazon-web-services-aws-authentication
source_filename: amazon-web-services-aws-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-web-services-aws-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request.\n  sources:\n  - openapi/amazon-web-services-aws-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/authentication/amazon-web-services-aws-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Artificial Intelligence
- Cloud Computing
- Computing
- Containers
- Databases
- Devops
- Iaas
- Infrastructure
- Machine-Learning
- Networking
- Paas
- Platform As A Service
- Security
- Serverless
- Storage
---
