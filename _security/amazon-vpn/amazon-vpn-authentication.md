---
api_key_in:
- header
api_specs:
- filename: amazon-vpn-openapi.yml
  format: yaml
  label: AWS VPN API
  slug: aws-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-vpn/refs/heads/main/openapi/amazon-vpn-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Vpn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon VPN secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon VPN
provider_slug: amazon-vpn
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request.
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/amazon-vpn-openapi.yml
  type: apiKey
slug: amazon-vpn-authentication
source_filename: amazon-vpn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-vpn-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request.\n  sources:\n  - openapi/amazon-vpn-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpn/refs/heads/main/authentication/amazon-vpn-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- Security
- VPN
---
