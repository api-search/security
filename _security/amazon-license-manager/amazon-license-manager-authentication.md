---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS License Manager API
  slug: aws-license-manager-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/license-manager/2018-08-01/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon License Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon License Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon License Manager
provider_slug: amazon-license-manager
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-license-manager-openapi.yml
  type: apiKey
slug: amazon-license-manager-authentication
source_filename: amazon-license-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-license-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-license-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-license-manager/refs/heads/main/authentication/amazon-license-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Cost Management
- License Management
- Software Licensing
---
