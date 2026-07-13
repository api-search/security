---
api_key_in:
- header
api_specs:
- filename: Welcome.html
  format: yaml
  label: AWS Organizations API
  slug: aws-organizations-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/organizations/latest/APIReference/Welcome.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Organizations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Organizations secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Organizations
provider_slug: amazon-organizations
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-organizations-openapi.yml
  type: apiKey
slug: amazon-organizations-authentication
source_filename: amazon-organizations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-organizations-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-organizations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/authentication/amazon-organizations-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Account Management
- Consolidated Billing
- Governance
- Multi-Account
- Organizations
- Policies
---
