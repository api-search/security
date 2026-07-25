---
api_key_in:
- header
api_specs:
- filename: amazon-application-migration-service-applications-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Applications API
  slug: amazon-application-migration-service-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-applications-api-openapi.yml
- filename: amazon-application-migration-service-exports-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Exports API
  slug: amazon-application-migration-service-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-exports-api-openapi.yml
- filename: amazon-application-migration-service-jobs-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Jobs API
  slug: amazon-application-migration-service-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-jobs-api-openapi.yml
- filename: amazon-application-migration-service-launch-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Launch API
  slug: amazon-application-migration-service-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-launch-api-openapi.yml
- filename: amazon-application-migration-service-lifecycle-hooks-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Lifecycle Hooks API
  slug: amazon-application-migration-service-lifecycle-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-lifecycle-hooks-api-openapi.yml
- filename: amazon-application-migration-service-replication-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Replication API
  slug: amazon-application-migration-service-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-replication-api-openapi.yml
- filename: amazon-application-migration-service-source-servers-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Source Servers API
  slug: amazon-application-migration-service-source-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-source-servers-api-openapi.yml
- filename: amazon-application-migration-service-tags-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Tags API
  slug: amazon-application-migration-service-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-tags-api-openapi.yml
- filename: amazon-application-migration-service-vcenter-clients-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Vcenter Clients API
  slug: amazon-application-migration-service-vcenter-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-vcenter-clients-api-openapi.yml
- filename: amazon-application-migration-service-waves-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Waves API
  slug: amazon-application-migration-service-waves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-waves-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Application Migration Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Application Migration Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsAuth
  parameter: Authorization
  sources:
  - openapi/amazon-application-migration-service-openapi.yml
  type: apiKey
slug: amazon-application-migration-service-authentication
source_filename: amazon-application-migration-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-application-migration-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-application-migration-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/authentication/amazon-application-migration-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
---
