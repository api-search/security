---
api_key_in:
- header
api_specs:
- filename: amazon-clean-rooms-openapi.yml
  format: yaml
  label: Amazon Clean Rooms API
  slug: amazon-clean-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/openapi/amazon-clean-rooms-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Clean Rooms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Clean Rooms secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-clean-rooms-openapi.yml
  type: apiKey
slug: amazon-clean-rooms-authentication
source_filename: amazon-clean-rooms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-clean-rooms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-clean-rooms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/authentication/amazon-clean-rooms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
---
