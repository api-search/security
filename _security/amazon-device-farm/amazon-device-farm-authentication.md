---
api_key_in:
- header
api_specs:
- filename: amazon-device-farm-openapi.yaml
  format: yaml
  label: AWS Device Farm API
  slug: aws-device-farm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/openapi/amazon-device-farm-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Device Farm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Device Farm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-device-farm-openapi.yaml
  type: apiKey
slug: amazon-device-farm-authentication
source_filename: amazon-device-farm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-device-farm-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-device-farm-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/authentication/amazon-device-farm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
---
