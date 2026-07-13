---
api_key_in:
- header
api_specs:
- filename: amazon-athena-openapi.yml
  format: yaml
  label: Amazon Athena API
  slug: amazon-athena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Athena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Athena secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Athena
provider_slug: amazon-athena
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-athena-openapi.yml
  type: apiKey
slug: amazon-athena-authentication
source_filename: amazon-athena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-athena-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-athena-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/authentication/amazon-athena-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Athena
- SQL
- Analytics
- Serverless
---
