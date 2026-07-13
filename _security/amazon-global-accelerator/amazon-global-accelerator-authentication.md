---
api_key_in:
- header
api_specs:
- filename: amazon-global-accelerator-openapi.yml
  format: yaml
  label: Amazon Global Accelerator API
  slug: amazon-global-accelerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/openapi/amazon-global-accelerator-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Global Accelerator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Global Accelerator secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-global-accelerator-openapi.yml
  type: apiKey
slug: amazon-global-accelerator-authentication
source_filename: amazon-global-accelerator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-global-accelerator-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-global-accelerator-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/authentication/amazon-global-accelerator-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
---
