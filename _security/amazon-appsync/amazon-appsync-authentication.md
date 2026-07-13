---
api_key_in:
- header
api_specs:
- filename: amazon-appsync-openapi.yml
  format: yaml
  label: Amazon AppSync API
  slug: amazon-appsync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Appsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon AppSync secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon AppSync
provider_slug: amazon-appsync
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsAuth
  parameter: Authorization
  sources:
  - openapi/amazon-appsync-openapi.yml
  type: apiKey
slug: amazon-appsync-authentication
source_filename: amazon-appsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-appsync-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-appsync-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/authentication/amazon-appsync-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
---
