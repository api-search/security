---
api_key_in: []
api_specs:
- filename: amazon-dynamodb-openapi.yml
  format: yaml
  label: Amazon DynamoDB API
  slug: amazon-dynamodb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Dynamodb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DynamoDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  name: sigv4Auth
  scheme: bearer
  sources:
  - openapi/amazon-dynamodb-openapi.yml
  type: http
slug: amazon-dynamodb-authentication
source_filename: amazon-dynamodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-dynamodb-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: sigv4Auth\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-dynamodb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/authentication/amazon-dynamodb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
---
