---
api_key_in:
- header
api_specs:
- filename: amazon-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml
  format: yaml
  label: Amazon Elastic Beanstalk Amazon Elastic Beanstalk AWS Elastic Beanstalk API API
  slug: amazon-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/openapi/amazon-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml
- filename: amazon-elastic-beanstalk-createenvironment-api-openapi.yml
  format: yaml
  label: 'Amazon Elastic Beanstalk #CreateEnvironment API'
  slug: amazon-elastic-beanstalk-createenvironment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/openapi/amazon-elastic-beanstalk-createenvironment-api-openapi.yml
- filename: amazon-elastic-beanstalk-describeenvironments-api-openapi.yml
  format: yaml
  label: 'Amazon Elastic Beanstalk #DescribeEnvironments API'
  slug: amazon-elastic-beanstalk-describeenvironments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/openapi/amazon-elastic-beanstalk-describeenvironments-api-openapi.yml
- filename: amazon-elastic-beanstalk-updateenvironment-api-openapi.yml
  format: yaml
  label: 'Amazon Elastic Beanstalk #UpdateEnvironment API'
  slug: amazon-elastic-beanstalk-updateenvironment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/openapi/amazon-elastic-beanstalk-updateenvironment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Elastic Beanstalk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Elastic Beanstalk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Elastic Beanstalk
provider_slug: amazon-elastic-beanstalk
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-elastic-beanstalk-openapi.yml
  type: apiKey
slug: amazon-elastic-beanstalk-authentication
source_filename: amazon-elastic-beanstalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-elastic-beanstalk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-elastic-beanstalk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/authentication/amazon-elastic-beanstalk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Auto Scaling
- Deployment
- Elastic Beanstalk
- PaaS
- Platform As A Service
- Web Applications
---
