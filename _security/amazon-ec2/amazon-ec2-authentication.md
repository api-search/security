---
api_key_in:
- header
api_specs:
- filename: amazon-ec2-openapi.yml
  format: yaml
  label: Amazon EC2 API
  slug: amazon-ec2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/openapi/amazon-ec2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ec2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EC2 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EC2
provider_slug: amazon-ec2
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-ec2-openapi.yml
  type: apiKey
slug: amazon-ec2-authentication
source_filename: amazon-ec2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ec2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-ec2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/authentication/amazon-ec2-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
---
