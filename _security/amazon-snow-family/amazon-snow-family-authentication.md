---
api_key_in:
- header
api_specs:
- filename: amazon-snow-family.yaml
  format: yaml
  label: AWS Snow Device Management API
  slug: aws-snow-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/openapi/amazon-snow-family.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Snow Family Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Snow Family secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-snow-family.yaml
  type: apiKey
slug: amazon-snow-family-authentication
source_filename: amazon-snow-family-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-snow-family.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-snow-family.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/authentication/amazon-snow-family-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
---
