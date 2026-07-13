---
api_key_in:
- header
api_specs:
- filename: amazon-workspaces-web-openapi-original.yaml
  format: yaml
  label: Amazon WorkSpaces Web API
  slug: amazon-workspaces-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Workspaces Web Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon WorkSpaces Web secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-workspaces-web-openapi-original.yaml
  type: apiKey
slug: amazon-workspaces-web-authentication
source_filename: amazon-workspaces-web-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-workspaces-web-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-workspaces-web-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/authentication/amazon-workspaces-web-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
---
