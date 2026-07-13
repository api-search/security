---
api_key_in:
- header
api_specs:
- filename: dynamodb-openapi.yml
  format: yaml
  label: Amazon DynamoDB API
  slug: amazon-dynamodb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-openapi.yml
- filename: dynamodb-streams-asyncapi.yml
  format: yaml
  label: Amazon DynamoDB Streams API
  slug: amazon-dynamodb-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/asyncapi/dynamodb-streams-asyncapi.yml
- filename: openapi.yaml
  format: yaml
  label: Amazon DynamoDB Accelerator (DAX) API
  slug: amazon-dynamodb-accelerator-dax-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/dax/2017-04-19/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dynamodb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DynamoDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DynamoDB
provider_slug: dynamodb
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. All DynamoDB requests must be signed using the AWS SigV4 signing process. The service name for signing is 'dynamodb'.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/dynamodb-openapi.yml
  type: apiKey
slug: dynamodb-authentication
source_filename: dynamodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dynamodb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. All DynamoDB requests must be signed\n    using the AWS SigV4 signing process. The service name for signing is 'dynamodb'.\n  sources:\n  - openapi/dynamodb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/authentication/dynamodb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
---
