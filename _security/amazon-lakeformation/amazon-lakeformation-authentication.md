---
api_key_in:
- header
api_specs:
- filename: amazon-lakeformation-openapi.yml
  format: yaml
  label: AWS Lake Formation API
  slug: aws-lake-formation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/openapi/amazon-lakeformation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Lakeformation Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Lake Formation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Lake Formation
provider_slug: amazon-lakeformation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-lakeformation-openapi.yml
  type: apiKey
slug: amazon-lakeformation-authentication
source_filename: amazon-lakeformation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-lakeformation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-lakeformation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/authentication/amazon-lakeformation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Data Lake
- Governance
---
