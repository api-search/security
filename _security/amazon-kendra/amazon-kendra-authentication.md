---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Kendra API
  slug: amazon-kendra-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kendra/2019-02-03/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kendra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Kendra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Kendra
provider_slug: amazon-kendra
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kendra-openapi.yml
  type: apiKey
slug: amazon-kendra-authentication
source_filename: amazon-kendra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kendra-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-kendra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/authentication/amazon-kendra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
---
