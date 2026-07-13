---
api_key_in:
- header
api_specs:
- filename: amazon-privatelink-openapi.yaml
  format: yaml
  label: AWS PrivateLink API
  slug: aws-privatelink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/openapi/amazon-privatelink-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Privatelink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon PrivateLink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-privatelink-openapi.yaml
  type: apiKey
slug: amazon-privatelink-authentication
source_filename: amazon-privatelink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-privatelink-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-privatelink-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/authentication/amazon-privatelink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
---
