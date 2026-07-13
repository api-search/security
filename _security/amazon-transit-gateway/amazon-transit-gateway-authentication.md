---
api_key_in:
- header
api_specs:
- filename: amazon-transit-gateway-openapi.yml
  format: yaml
  label: Amazon Transit Gateway REST API
  slug: amazon-transit-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-transit-gateway/refs/heads/main/openapi/amazon-transit-gateway-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Transit Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Transit Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Transit Gateway
provider_slug: amazon-transit-gateway
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-transit-gateway-openapi.yml
  type: apiKey
slug: amazon-transit-gateway-authentication
source_filename: amazon-transit-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-transit-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-transit-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-transit-gateway/refs/heads/main/authentication/amazon-transit-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Networking
- Network Hub
- Networking
- Transit Gateway
- VPC
---
