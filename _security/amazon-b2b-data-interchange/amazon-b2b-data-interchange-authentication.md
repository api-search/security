---
api_key_in:
- header
api_specs:
- filename: aws-b2b-data-interchange-api-openapi.yml
  format: yaml
  label: AWS B2B Data Interchange API
  slug: aws-b2b-data-interchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/aws-b2b-data-interchange-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon B2B Data Interchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon B2B Data Interchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_iam
  parameter: Authorization
  sources:
  - openapi/aws-b2b-data-interchange-api-openapi.yml
  type: apiKey
slug: amazon-b2b-data-interchange-authentication
source_filename: amazon-b2b-data-interchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-b2b-data-interchange-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_iam\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/aws-b2b-data-interchange-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/authentication/amazon-b2b-data-interchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial Services
- Amazon Web Services
---
