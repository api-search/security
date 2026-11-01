---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-documentdb-amazon-documentdb-api-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Amazon DocumentDB API
  slug: amazon-documentdb-amazon-documentdb-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-amazon-documentdb-api-api-openapi.yml
- filename: amazon-documentdb-db-cluster-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Db Cluster API
  slug: amazon-documentdb-db-cluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-db-cluster-api-openapi.yml
- filename: amazon-documentdb-db-cluster-parameter-group-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Db Cluster Parameter Group API
  slug: amazon-documentdb-db-cluster-parameter-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-db-cluster-parameter-group-api-openapi.yml
- filename: amazon-documentdb-db-cluster-snapshot-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Db Cluster Snapshot API
  slug: amazon-documentdb-db-cluster-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-db-cluster-snapshot-api-openapi.yml
- filename: amazon-documentdb-db-subnet-group-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Db Subnet Group API
  slug: amazon-documentdb-db-subnet-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-db-subnet-group-api-openapi.yml
- filename: amazon-documentdb-event-subscription-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Event Subscription API
  slug: amazon-documentdb-event-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-event-subscription-api-openapi.yml
- filename: amazon-documentdb-global-cluster-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Global Cluster API
  slug: amazon-documentdb-global-cluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-global-cluster-api-openapi.yml
- filename: amazon-documentdb-operations-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Operations API
  slug: amazon-documentdb-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-operations-api-openapi.yml
- filename: amazon-documentdb-tag-api-openapi.yml
  format: yaml
  label: Amazon DocumentDB Documentdb Tag API
  slug: amazon-documentdb-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-documentdb/openapi/amazon-documentdb-tag-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Documentdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DocumentDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-documentdb-openapi.yml
  type: apiKey
slug: amazon-documentdb-authentication
source_filename: amazon-documentdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-documentdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-documentdb-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-documentdb/authentication/amazon-documentdb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
---
