---
api_key_in:
- header
api_specs:
- filename: amazon-waf-openapi.yml
  format: yaml
  label: Amazon WAF REST API
  slug: amazon-waf-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-waf/refs/heads/main/openapi/amazon-waf-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Waf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon WAF secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon WAF
provider_slug: amazon-waf
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-waf-openapi.yml
  type: apiKey
slug: amazon-waf-authentication
source_filename: amazon-waf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-waf-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-waf-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-waf/refs/heads/main/authentication/amazon-waf-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bot Management
- Ddos Protection
- Security
- WAF
- Web Application Firewall
---
