---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-timestream-databases-api-openapi.yml
  format: yaml
  label: Amazon Timestream Databases API
  slug: amazon-timestream-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-databases-api-openapi.yml
- filename: amazon-timestream-query-api-openapi.yml
  format: yaml
  label: Amazon Timestream Query API
  slug: amazon-timestream-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-query-api-openapi.yml
- filename: amazon-timestream-tables-api-openapi.yml
  format: yaml
  label: Amazon Timestream Tables API
  slug: amazon-timestream-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-tables-api-openapi.yml
- filename: amazon-timestream-write-api-openapi.yml
  format: yaml
  label: Amazon Timestream Write API
  slug: amazon-timestream-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-write-api-openapi.yml
- filename: amazon-timestream-batch-load-task-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Batch Load Task API
  slug: amazon-timestream-batch-load-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-batch-load-task-api-openapi.yml
- filename: amazon-timestream-operations-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Operations API
  slug: amazon-timestream-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-operations-api-openapi.yml
- filename: amazon-timestream-scheduled-query-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Scheduled Query API
  slug: amazon-timestream-scheduled-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-scheduled-query-api-openapi.yml
- filename: amazon-timestream-db-backup-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Db Backup API
  slug: amazon-timestream-db-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-db-backup-api-openapi.yml
- filename: amazon-timestream-db-cluster-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Db Cluster API
  slug: amazon-timestream-db-cluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-db-cluster-api-openapi.yml
- filename: amazon-timestream-db-instance-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Db Instance API
  slug: amazon-timestream-db-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-db-instance-api-openapi.yml
- filename: amazon-timestream-db-parameter-group-api-openapi.yml
  format: yaml
  label: Amazon Timestream Timestream Db Parameter Group API
  slug: amazon-timestream-db-parameter-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-timestream/openapi/amazon-timestream-db-parameter-group-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Timestream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Timestream secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Timestream
provider_slug: amazon-timestream
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-timestream-batch-load-task-api-openapi.yml
  - openapi/amazon-timestream-databases-api-openapi.yml
  - openapi/amazon-timestream-db-backup-api-openapi.yml
  - openapi/amazon-timestream-db-cluster-api-openapi.yml
  - openapi/amazon-timestream-db-instance-api-openapi.yml
  - openapi/amazon-timestream-db-parameter-group-api-openapi.yml
  - openapi/amazon-timestream-operations-api-openapi.yml
  - openapi/amazon-timestream-query-api-openapi.yml
  - openapi/amazon-timestream-scheduled-query-api-openapi.yml
  - openapi/amazon-timestream-tables-api-openapi.yml
  - openapi/amazon-timestream-write-api-openapi.yml
  type: apiKey
slug: amazon-timestream-authentication
source_filename: amazon-timestream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-timestream-batch-load-task-api-openapi.yml, openapi/amazon-timestream-databases-api-openapi.yml,\n  openapi/amazon-timestream-db-backup-api-openapi.yml, openapi/amazon-timestream-db-cluster-api-openapi.yml,\n  openapi/amazon-timestream-db-instance-api-openapi.yml, openapi/amazon-timestream-db-parameter-group-api-openapi.yml,\n  openapi/amazon-timestream-operations-api-openapi.yml, openapi/amazon-timestream-query-api-openapi.yml,\n  openapi/amazon-timestream-scheduled-query-api-openapi.yml, openapi/amazon-timestream-tables-api-openapi.yml,\n  openapi/amazon-timestream-write-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n\
  \    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-timestream-batch-load-task-api-openapi.yml\n  - openapi/amazon-timestream-databases-api-openapi.yml\n  - openapi/amazon-timestream-db-backup-api-openapi.yml\n  - openapi/amazon-timestream-db-cluster-api-openapi.yml\n  - openapi/amazon-timestream-db-instance-api-openapi.yml\n  - openapi/amazon-timestream-db-parameter-group-api-openapi.yml\n  - openapi/amazon-timestream-operations-api-openapi.yml\n  - openapi/amazon-timestream-query-api-openapi.yml\n  - openapi/amazon-timestream-scheduled-query-api-openapi.yml\n  - openapi/amazon-timestream-tables-api-openapi.yml\n  - openapi/amazon-timestream-write-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-timestream/authentication/amazon-timestream-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Database
- IoT
- Time Series
---
