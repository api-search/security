---
api_key_in:
- header
api_specs:
- filename: amazon-vpc-openapi.yml
  format: yaml
  label: Amazon VPC API
  slug: amazon-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/openapi/amazon-vpc-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Vpc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon VPC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon VPC
provider_slug: amazon-vpc
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-vpc-openapi.yml
  type: apiKey
slug: amazon-vpc-authentication
source_filename: amazon-vpc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-vpc-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-vpc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/authentication/amazon-vpc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
---
