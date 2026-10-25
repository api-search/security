---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amazon-dynamodb-batch-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Batch API
  slug: amazon-dynamodb-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-batch-api-openapi.yml
- filename: amazon-dynamodb-items-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Items API
  slug: amazon-dynamodb-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-items-api-openapi.yml
- filename: amazon-dynamodb-queries-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Queries API
  slug: amazon-dynamodb-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-queries-api-openapi.yml
- filename: amazon-dynamodb-tables-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Tables API
  slug: amazon-dynamodb-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-tables-api-openapi.yml
- filename: amazon-dynamodb-transactions-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Transactions API
  slug: amazon-dynamodb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-transactions-api-openapi.yml
- filename: amazon-dynamodb-backups-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Backups API
  slug: amazon-dynamodb-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-backups-api-openapi.yml
- filename: amazon-dynamodb-contributor-insights-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Contributor Insights API
  slug: amazon-dynamodb-contributor-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-contributor-insights-api-openapi.yml
- filename: amazon-dynamodb-exports-imports-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Exports Imports API
  slug: amazon-dynamodb-exports-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-exports-imports-api-openapi.yml
- filename: amazon-dynamodb-global-tables-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Global Tables API
  slug: amazon-dynamodb-global-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-global-tables-api-openapi.yml
- filename: amazon-dynamodb-operations-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Operations API
  slug: amazon-dynamodb-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-operations-api-openapi.yml
- filename: amazon-dynamodb-resource-policies-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Resource Policies API
  slug: amazon-dynamodb-resource-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-resource-policies-api-openapi.yml
- filename: amazon-dynamodb-streams-kinesis-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Streams Kinesis API
  slug: amazon-dynamodb-streams-kinesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-streams-kinesis-api-openapi.yml
- filename: amazon-dynamodb-tags-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Tags API
  slug: amazon-dynamodb-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-tags-api-openapi.yml
- filename: amazon-dynamodb-ttl-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Dynamodb Ttl API
  slug: amazon-dynamodb-ttl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/openapi/amazon-dynamodb-ttl-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
  - openapi/amazon-dynamodb-batch-api-openapi.yml
  - openapi/amazon-dynamodb-items-api-openapi.yml
  - openapi/amazon-dynamodb-queries-api-openapi.yml
  - openapi/amazon-dynamodb-tables-api-openapi.yml
  - openapi/amazon-dynamodb-transactions-api-openapi.yml
  type: http
slug: amazon-dynamodb-authentication
source_filename: amazon-dynamodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/amazon-dynamodb-batch-api-openapi.yml, openapi/amazon-dynamodb-items-api-openapi.yml,\n  openapi/amazon-dynamodb-queries-api-openapi.yml, openapi/amazon-dynamodb-tables-api-openapi.yml,\n  openapi/amazon-dynamodb-transactions-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: sigv4Auth\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-dynamodb-batch-api-openapi.yml\n  - openapi/amazon-dynamodb-items-api-openapi.yml\n  - openapi/amazon-dynamodb-queries-api-openapi.yml\n  - openapi/amazon-dynamodb-tables-api-openapi.yml\n  - openapi/amazon-dynamodb-transactions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/authentication/amazon-dynamodb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Document Store
- Key-Value Store
- NoSQL
- Serverless
---
