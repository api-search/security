---
api_key_in:
- header
api_specs:
- filename: amazon-mainframe-modernization-openapi-original.yaml
  format: yaml
  label: AWS Mainframe Modernization API
  slug: aws-mainframe-modernization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/openapi/amazon-mainframe-modernization-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mainframe Modernization Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Mainframe Modernization secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mainframe-modernization-openapi-original.yaml
  type: apiKey
slug: amazon-mainframe-modernization-authentication
source_filename: amazon-mainframe-modernization-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mainframe-modernization-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mainframe-modernization-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/authentication/amazon-mainframe-modernization-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
---
