---
api_key_in:
- header
api_specs:
- filename: amazon-network-firewall-openapi.yml
  format: yaml
  label: AWS Network Firewall API
  slug: aws-network-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/openapi/amazon-network-firewall-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Network Firewall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Network Firewall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-network-firewall-openapi.yml
  type: apiKey
slug: amazon-network-firewall-authentication
source_filename: amazon-network-firewall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-network-firewall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-network-firewall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/authentication/amazon-network-firewall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
---
