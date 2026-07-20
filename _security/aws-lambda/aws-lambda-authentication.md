---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: AWS Lambda API
  slug: aws-lambda-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/lambda/2015-03-31/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aws Lambda Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Lambda secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Lambda
provider_slug: aws-lambda
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed with valid AWS credentials that have the appropriate Lambda IAM permissions.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/aws-lambda-api-openapi.yml
  type: apiKey
slug: aws-lambda-authentication
source_filename: aws-lambda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/aws-lambda-api-openapi.yml\ndocs: https://docs.aws.amazon.com/lambda/latest/dg/security-iam.html\nsigning_docs: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_sigv.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Requests must be signed with valid AWS\n    credentials that have the appropriate Lambda IAM permissions.\n  sources:\n  - openapi/aws-lambda-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/authentication/aws-lambda-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
