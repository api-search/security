---
api_key_in:
- header
api_specs:
- filename: amazon-codecatalyst-openapi-original.yaml
  format: yaml
  label: Amazon CodeCatalyst API
  slug: amazon-codecatalyst-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/openapi/amazon-codecatalyst-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Codecatalyst Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeCatalyst secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
scheme_count: 1
schemes:
- in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codecatalyst-openapi-original.yaml
  type: apiKey
slug: amazon-codecatalyst-authentication
source_filename: amazon-codecatalyst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codecatalyst-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/amazon-codecatalyst-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/authentication/amazon-codecatalyst-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
---
