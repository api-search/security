---
api_key_in:
- header
api_specs:
- filename: amazon-codestar-openapi.yml
  format: yaml
  label: AWS CodeStar API
  slug: aws-codestar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/openapi/amazon-codestar-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Codestar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeStar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codestar-openapi.yml
  type: apiKey
slug: amazon-codestar-authentication
source_filename: amazon-codestar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codestar-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codestar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/authentication/amazon-codestar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
---
