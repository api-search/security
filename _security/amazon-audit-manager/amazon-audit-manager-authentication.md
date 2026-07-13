---
api_key_in:
- header
api_specs:
- filename: amazon-audit-manager-openapi.yml
  format: yaml
  label: Amazon Audit Manager API
  slug: amazon-audit-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Audit Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Audit Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Audit Manager
provider_slug: amazon-audit-manager
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-audit-manager-openapi.yml
  type: apiKey
slug: amazon-audit-manager-authentication
source_filename: amazon-audit-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-audit-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-audit-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/authentication/amazon-audit-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Audit Manager
- Compliance
- Audit
- Risk Management
---
