---
api_key_in:
- header
api_specs:
- filename: amazon-serverless-application-repository-openapi.yml
  format: yaml
  label: AWS Serverless Application Repository API
  slug: aws-serverless-application-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/openapi/amazon-serverless-application-repository-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Serverless Application Repository Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Serverless Application Repository secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Serverless Application Repository
provider_slug: amazon-serverless-application-repository
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: AWSSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-serverless-application-repository-openapi.yml
  type: apiKey
slug: amazon-serverless-application-repository-authentication
source_filename: amazon-serverless-application-repository-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-serverless-application-repository-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWSSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-serverless-application-repository-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/authentication/amazon-serverless-application-repository-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Repository
- Lambda
- SAM
- Serverless
---
