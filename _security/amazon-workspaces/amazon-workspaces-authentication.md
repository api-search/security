---
api_key_in:
- header
api_specs:
- filename: amazon-workspaces-openapi-original.yaml
  format: yaml
  label: Amazon WorkSpaces API
  slug: amazon-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/openapi/amazon-workspaces-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Workspaces Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon WorkSpaces secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-workspaces-openapi-original.yaml
  type: apiKey
slug: amazon-workspaces-authentication
source_filename: amazon-workspaces-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-workspaces-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-workspaces-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/authentication/amazon-workspaces-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
---
