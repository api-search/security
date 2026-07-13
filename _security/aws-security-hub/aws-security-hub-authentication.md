---
api_key_in:
- header
api_specs:
- filename: aws-security-hub-openapi.yml
  format: yaml
  label: AWS Security Hub CSPM API
  slug: cspm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Security Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Security Hub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Security Hub
provider_slug: aws-security-hub
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-security-hub-openapi.yml
  type: apiKey
slug: aws-security-hub-authentication
source_filename: aws-security-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-security-hub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-security-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/authentication/aws-security-hub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Cloud Security Posture Management
- Compliance
- Findings
- Threat Detection
- Cloud
---
