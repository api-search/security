---
api_key_in:
- header
api_specs:
- filename: amazon-glue-openapi.yml
  format: yaml
  label: Amazon Glue API
  slug: amazon-glue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/openapi/amazon-glue-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Glue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Glue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Glue
provider_slug: amazon-glue
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-glue-openapi.yml
  type: apiKey
slug: amazon-glue-authentication
source_filename: amazon-glue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-glue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-glue-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/authentication/amazon-glue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
---
