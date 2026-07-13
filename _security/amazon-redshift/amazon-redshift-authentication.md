---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Redshift API
  slug: amazon-redshift-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/redshift/2012-12-01/openapi.yaml
- filename: amazon-redshift-data-api-openapi.yml
  format: yaml
  label: Amazon Redshift Data API
  slug: amazon-redshift-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Redshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Redshift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Redshift
provider_slug: amazon-redshift
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests are signed using IAM credentials. The Data API also supports authentication via AWS Secrets Manager for database credentials or temporary IAM credentials.
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-redshift-data-api-openapi.yml
  type: apiKey
slug: amazon-redshift-authentication
source_filename: amazon-redshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-redshift-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Requests are signed using IAM credentials.\n    The Data API also supports authentication via AWS Secrets Manager for database credentials\n    or temporary IAM credentials.\n  sources:\n  - openapi/amazon-redshift-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/authentication/amazon-redshift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
---
