---
api_key_in:
- header
api_specs:
- filename: dynamodb-streams-asyncapi.yml
  format: yaml
  label: Amazon DynamoDB Streams API
  slug: amazon-dynamodb-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/asyncapi/dynamodb-streams-asyncapi.yml
- filename: dynamodb-backups-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Backups API
  slug: dynamodb-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-backups-api-openapi.yml
- filename: dynamodb-batch-operations-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Batch Operations API
  slug: dynamodb-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-batch-operations-api-openapi.yml
- filename: dynamodb-exports-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Exports API
  slug: dynamodb-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-exports-api-openapi.yml
- filename: dynamodb-imports-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Imports API
  slug: dynamodb-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-imports-api-openapi.yml
- filename: dynamodb-items-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Items API
  slug: dynamodb-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-items-api-openapi.yml
- filename: dynamodb-listtagsofresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #ListTagsOfResource API'
  slug: dynamodb-listtagsofresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-listtagsofresource-api-openapi.yml
- filename: dynamodb-partiql-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB PartiQL API
  slug: dynamodb-partiql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-partiql-api-openapi.yml
- filename: dynamodb-queries-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Queries API
  slug: dynamodb-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-queries-api-openapi.yml
- filename: dynamodb-tables-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Tables API
  slug: dynamodb-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-tables-api-openapi.yml
- filename: dynamodb-tagresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #TagResource API'
  slug: dynamodb-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-tagresource-api-openapi.yml
- filename: dynamodb-transactions-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Transactions API
  slug: dynamodb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-transactions-api-openapi.yml
- filename: dynamodb-ttl-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB TTL API
  slug: dynamodb-ttl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-ttl-api-openapi.yml
- filename: dynamodb-untagresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #UntagResource API'
  slug: dynamodb-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-untagresource-api-openapi.yml
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
