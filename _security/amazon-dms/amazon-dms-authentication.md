---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-dms-endpoints-api-openapi.yml
  format: yaml
  label: Amazon DMS Endpoints API
  slug: amazon-dms-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/openapi/amazon-dms-endpoints-api-openapi.yml
- filename: amazon-dms-replication-instances-api-openapi.yml
  format: yaml
  label: Amazon DMS Replication Instances API
  slug: amazon-dms-replication-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/openapi/amazon-dms-replication-instances-api-openapi.yml
- filename: amazon-dms-replication-tasks-api-openapi.yml
  format: yaml
  label: Amazon DMS Replication Tasks API
  slug: amazon-dms-replication-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/openapi/amazon-dms-replication-tasks-api-openapi.yml
- filename: amazon-dms-aws-database-migration-service-api-openapi.yml
  format: yaml
  label: Amazon DMS AWS Database Migration Service API
  slug: amazon-dms-aws-database-migration-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/openapi/amazon-dms-aws-database-migration-service-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Dms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DMS
provider_slug: amazon-dms
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-dms-openapi.yaml
  type: apiKey
slug: amazon-dms-authentication
source_filename: amazon-dms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-dms-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-dms-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/authentication/amazon-dms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Replication
- Database
- Database Migration
- Migration
---
