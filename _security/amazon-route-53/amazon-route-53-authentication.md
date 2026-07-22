---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Route 53 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Route 53 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Route 53
provider_slug: amazon-route-53
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-route-53-openapi.yml
  type: apiKey
slug: amazon-route-53-authentication
source_filename: amazon-route-53-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-route-53-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-route-53-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-route-53/refs/heads/main/authentication/amazon-route-53-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Domain Registration
- Health Checks
- Routing
---
