---
api_key_in:
- header
api_specs:
- filename: amazon-entity-resolution-openapi.yml
  format: yaml
  label: Amazon Entity Resolution API
  slug: amazon-entity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/openapi/amazon-entity-resolution-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Entity Resolution Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Entity Resolution secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-entity-resolution-openapi.yml
  type: apiKey
slug: amazon-entity-resolution-authentication
source_filename: amazon-entity-resolution-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-entity-resolution-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-entity-resolution-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/authentication/amazon-entity-resolution-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
---
