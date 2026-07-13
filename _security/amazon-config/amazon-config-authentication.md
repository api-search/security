---
api_key_in:
- header
api_specs:
- filename: amazon-config-openapi.yml
  format: yaml
  label: Amazon Config API
  slug: amazon-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/openapi/amazon-config-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Config Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Config secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Config
provider_slug: amazon-config
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-config-openapi.yml
  type: apiKey
slug: amazon-config-authentication
source_filename: amazon-config-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-config-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-config-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/authentication/amazon-config-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
---
