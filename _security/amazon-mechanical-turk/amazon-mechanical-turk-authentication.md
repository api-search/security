---
api_key_in:
- header
api_specs:
- filename: amazon-mechanical-turk-openapi-original.yaml
  format: yaml
  label: Amazon Mechanical Turk API
  slug: amazon-mturk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/openapi/amazon-mechanical-turk-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mechanical Turk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Mechanical Turk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mechanical-turk-openapi-original.yaml
  type: apiKey
slug: amazon-mechanical-turk-authentication
source_filename: amazon-mechanical-turk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mechanical-turk-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mechanical-turk-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/authentication/amazon-mechanical-turk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
---
