---
api_key_in:
- header
api_specs:
- filename: amazon-ec2-auto-scaling-openapi.yaml
  format: yaml
  label: Amazon EC2 Auto Scaling API
  slug: amazon-ec2-auto-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/openapi/amazon-ec2-auto-scaling-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ec2 Auto Scaling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EC2 Auto Scaling secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-ec2-auto-scaling-openapi.yaml
  type: apiKey
slug: amazon-ec2-auto-scaling-authentication
source_filename: amazon-ec2-auto-scaling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ec2-auto-scaling-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-ec2-auto-scaling-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/authentication/amazon-ec2-auto-scaling-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
---
