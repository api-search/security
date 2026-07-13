---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Launch Wizard API
  slug: aws-launch-wizard-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/launchwizard/2018-05-10/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Launch Wizard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Launch Wizard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Launch Wizard
provider_slug: amazon-launch-wizard
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-launch-wizard-openapi.yml
  type: apiKey
slug: amazon-launch-wizard-authentication
source_filename: amazon-launch-wizard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-launch-wizard-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-launch-wizard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-launch-wizard/refs/heads/main/authentication/amazon-launch-wizard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Deployment
- Enterprise Applications
- SAP
- SQL Server
---
