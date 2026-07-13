---
api_key_in:
- header
api_specs:
- filename: amazon-well-architected-tool-openapi-original.yaml
  format: yaml
  label: AWS Well-Architected Tool API
  slug: aws-well-architected-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Well Architected Tool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Well-Architected Tool secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-well-architected-tool-openapi-original.yaml
  type: apiKey
slug: amazon-well-architected-tool-authentication
source_filename: amazon-well-architected-tool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-well-architected-tool-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-well-architected-tool-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/authentication/amazon-well-architected-tool-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
---
