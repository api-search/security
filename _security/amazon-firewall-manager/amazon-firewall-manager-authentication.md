---
api_key_in:
- header
api_specs:
- filename: amazon-firewall-manager-openapi.yml
  format: yaml
  label: AWS Firewall Manager API
  slug: aws-firewall-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/openapi/amazon-firewall-manager-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Firewall Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Firewall Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/amazon-firewall-manager-openapi.yml
  type: apiKey
slug: amazon-firewall-manager-authentication
source_filename: amazon-firewall-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-firewall-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-firewall-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/authentication/amazon-firewall-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Firewall
- Network Security
- Security
---
