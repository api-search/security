---
api_key_in:
- header
api_specs:
- filename: amazon-glue-databrew-openapi.yaml
  format: yaml
  label: AWS Glue DataBrew API
  slug: aws-glue-databrew-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Glue Databrew Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Glue DataBrew secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-glue-databrew-openapi.yaml
  type: apiKey
slug: amazon-glue-databrew-authentication
source_filename: amazon-glue-databrew-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-glue-databrew-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-glue-databrew-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/authentication/amazon-glue-databrew-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
---
