---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-elasticache-amazon-elasticache-api-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Amazon ElastiCache API
  slug: amazon-elasticache-amazon-elasticache-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-amazon-elasticache-api-api-openapi.yml
- filename: amazon-elasticache-cache-parameter-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Parameter Group API
  slug: amazon-elasticache-cache-parameter-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-parameter-group-api-openapi.yml
- filename: amazon-elasticache-cache-security-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Security Group API
  slug: amazon-elasticache-cache-security-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-security-group-api-openapi.yml
- filename: amazon-elasticache-cache-subnet-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Subnet Group API
  slug: amazon-elasticache-cache-subnet-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-subnet-group-api-openapi.yml
- filename: amazon-elasticache-global-replication-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Global Replication Group API
  slug: amazon-elasticache-global-replication-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-global-replication-group-api-openapi.yml
- filename: amazon-elasticache-migration-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Migration API
  slug: amazon-elasticache-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-migration-api-openapi.yml
- filename: amazon-elasticache-operations-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Operations API
  slug: amazon-elasticache-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-operations-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache API
  slug: amazon-elasticache-serverless-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache Snapshot API
  slug: amazon-elasticache-serverless-cache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
- filename: amazon-elasticache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Snapshot API
  slug: amazon-elasticache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-snapshot-api-openapi.yml
- filename: amazon-elasticache-tag-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Tag API
  slug: amazon-elasticache-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-tag-api-openapi.yml
- filename: amazon-elasticache-update-action-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Update Action API
  slug: amazon-elasticache-update-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-update-action-api-openapi.yml
- filename: amazon-elasticache-user-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User API
  slug: amazon-elasticache-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-api-openapi.yml
- filename: amazon-elasticache-user-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User Group API
  slug: amazon-elasticache-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-group-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Elasticache Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon ElastiCache secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-elasticache-openapi.yml
  type: apiKey
slug: amazon-elasticache-authentication
source_filename: amazon-elasticache-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-elasticache-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-elasticache-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-elasticache/authentication/amazon-elasticache-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
---
