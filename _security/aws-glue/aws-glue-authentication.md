---
api_key_in:
- header
api_specs:
- filename: aws-glue-openapi.yml
  format: yaml
  label: AWS Glue API
  slug: glue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-glue/refs/heads/main/openapi/aws-glue-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Glue Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Glue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Glue
provider_slug: aws-glue
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-glue-openapi.yml
  type: apiKey
slug: aws-glue-authentication
source_filename: aws-glue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-glue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-glue-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-glue/refs/heads/main/authentication/aws-glue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data
- Data Catalog
- ETL
- Analytics
- Serverless
---
