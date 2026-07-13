---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Lake Formation API
  slug: amazon-lake-formation-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/lakeformation/2017-03-31/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Lake Formation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lake Formation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lake Formation
provider_slug: amazon-lake-formation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-lake-formation-openapi.yml
  type: apiKey
slug: amazon-lake-formation-authentication
source_filename: amazon-lake-formation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-lake-formation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-lake-formation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lake-formation/refs/heads/main/authentication/amazon-lake-formation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Control
- Analytics
- Data Governance
- Data Lake
- S3
---
