---
api_key_in:
- header
api_specs:
- filename: amazon-cloud-wan-openapi.yml
  format: yaml
  label: Amazon Cloud WAN API
  slug: amazon-cloud-wan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/openapi/amazon-cloud-wan-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Cloud Wan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Cloud WAN secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-cloud-wan-openapi.yml
  type: apiKey
slug: amazon-cloud-wan-authentication
source_filename: amazon-cloud-wan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloud-wan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-cloud-wan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/authentication/amazon-cloud-wan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
---
