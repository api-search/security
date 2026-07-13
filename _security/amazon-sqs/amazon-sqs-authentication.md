---
api_key_in:
- header
api_specs:
- filename: amazon-sqs-openapi.yml
  format: yaml
  label: Amazon SQS API
  slug: amazon-sqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/openapi/amazon-sqs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Sqs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SQS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SQS
provider_slug: amazon-sqs
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. All SQS API requests must be signed using AWS credentials (Access Key ID and Secret Access Key). The signature is included in the Authorization header.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-sqs-openapi.yml
  type: apiKey
slug: amazon-sqs-authentication
source_filename: amazon-sqs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-sqs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. All SQS API requests must be signed using\n    AWS credentials (Access Key ID and Secret Access Key). The signature is included in the\n    Authorization header.\n  sources:\n  - openapi/amazon-sqs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/authentication/amazon-sqs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud
- Distributed Systems
- Messaging
- Microservices
- Queue
---
