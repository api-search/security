---
api_key_in:
- header
api_specs:
- filename: amazon-aurora-dsql-openapi.yml
  format: yaml
  label: Amazon Aurora DSQL API
  slug: amazon-aurora-dsql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora-dsql/refs/heads/main/openapi/amazon-aurora-dsql-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Aurora Dsql Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Aurora DSQL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Aurora DSQL
provider_slug: amazon-aurora-dsql
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-aurora-dsql-openapi.yml
  type: apiKey
slug: amazon-aurora-dsql-authentication
source_filename: amazon-aurora-dsql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-aurora-dsql-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-aurora-dsql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora-dsql/refs/heads/main/authentication/amazon-aurora-dsql-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Aurora DSQL
- Distributed SQL
- PostgreSQL
- Serverless
---
