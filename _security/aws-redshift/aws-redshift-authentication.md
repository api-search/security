---
api_key_in:
- header
api_specs:
- filename: aws-redshift-openapi.json
  format: json
  label: Amazon Redshift API
  slug: amazon-redshift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/openapi/aws-redshift-openapi.json
- filename: aws-redshift-data-openapi.json
  format: json
  label: Amazon Redshift Data API
  slug: amazon-redshift-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/openapi/aws-redshift-data-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Redshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Redshift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Redshift
provider_slug: aws-redshift
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-redshift-data-openapi.json
  - openapi/aws-redshift-openapi.json
  type: apiKey
slug: aws-redshift-authentication
source_filename: aws-redshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-redshift-data-openapi.json, openapi/aws-redshift-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/aws-redshift-data-openapi.json\n  - openapi/aws-redshift-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/authentication/aws-redshift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
---
