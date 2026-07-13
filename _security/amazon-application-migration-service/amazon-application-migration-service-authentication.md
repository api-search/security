---
api_key_in:
- header
api_specs:
- filename: amazon-application-migration-service-openapi.yml
  format: yaml
  label: Amazon Application Migration Service API
  slug: amazon-application-migration-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-openapi.yml
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
